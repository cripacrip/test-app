<template>
    <div class="resume__reviews">
        <div
            class="resume__reviews-lol"
            id="comm-list"
        >
            <div
                class="resume__reviews-part"
                v-for="list in lists"
                :key="list.id"
                :title="list.title"
                :data="list.data"
                :name="list.name"
            >
                <div class="resume__reviews-info">
                    <div
                        class="resume__reviews-name"
                    >
                        {{ list.name }}
                    </div>
                    <div
                        class="resume__reviews-date"
                    >
                        {{ list.date }}
                    </div>
                </div>
                <div
                    class="resume__reviews-comment"
                >
                   {{ list.title }}
            </div>
        </div>
        <div class="resume__reviews-form">
            <form
                class="form"
                v-on:submit.prevent="addNewComm">
                <input
                    class="input"
                    type="text"
                    v-model="addComm"
                >
                <button class="button">Написать консультанту</button>
            </form>
        </div>
        </div>
    </div>
</template>

<script>
export default {
    data: () => ({
        addComm: '',
        lists: [
            {
                'id': 1,
                'title': ' Привет, Верунь! ниче себе ты крутая. фотка класс!!!!',
                'name': 'Самуил',
                'date': '13 октября 2011'
            },
           {
                'id': 2,
                'title': 'Вероника, здравствуйте! Есть такой вопрос: Особый вид куниц жизненно стабилизирует кинетический момент, это и есть всемирно известный центр огранки алмазов и торговли бриллиантами?',
                'name': 'Лилия Семенова',
                'date': '14 октября 2011'
            },
           {
                'id': 3,
                'title': 'Вероника, здравствуйте! Есть такой вопрос: Особый вид куниц жизненно стабилизирует кинетический момент?',
                'name': 'Лилия Семенова',
                'date': '14 октября 2011'
            },
        ],
        nextCommId: 4
    }),
    methods: {
        addNewComm() {
            this.lists.push({
                id: this.nextCommId++,
                title: this.addComm
            })
            this.addComm = ''
        }
    }
}
</script>

<style>
.resume__reviews-lol {
    margin-bottom: 22px;
}
.resume__reviews-part {
  margin-top: 16px;
}
.resume__reviews-info {
  display: flex;
}
.resume__reviews-name {
  font-weight: bold;
  font-size: 16px;
  line-height: 20px;

  padding-right: 10px;
}
.resume__reviews-date {
  font-size: 12px;
  line-height: 20px;
  color: #808080;
}
.resume__reviews-comment {
	position: relative;
    background-color: #F2FBFF;
    padding: 13px;
	border: 1px solid #C4CBCF;
    margin-top: 10px;

    font-size: 14px;
    line-height: 19px;
}
.resume__reviews-comment:before {
	content: ' ';
	position: absolute;
	width: 0;
	height: 0;
    left: 23px;
    top: -15px;
    border: 7px solid;
    border-color: transparent transparent #C4CBCF #C4CBCF;
}
.resume__reviews-comment:after {
    content: ' ';
	position: absolute;
	width: 0;
	height: 0;
    left: 24px;
    top: -13px;
    border: 7px solid;
    border-color: transparent transparent #F2FBFF #F2FBFF;
}
.resume__reviews-form {
    background-color: #F2F2F2;
}
.form {
    display: flex;
    flex-direction: column;
    margin-top: 22px;
}
.input {
    margin: 28px 21px 23px;
    height: 63px;
}
.button {
    margin: auto;
    max-width: 281px;
    margin-bottom: 34px;
    padding: 13px 45px;
    background: #FDD639;
    border-radius: 23px;
    font-family: PT Sans;
    font-weight: bold;
    font-size: 16px;
    line-height: 21px;
}
</style>