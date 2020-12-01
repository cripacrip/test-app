<template>
    <div class="resume__services">
        <div class="resume__services-name">Услуги</div>
        <div class="resume__services-scroll">
          <div class="resume__servise-left">
            <div class="resume__services-booking">
              <p>
                Ручное пронировани
              </p>
            </div>
            <div class="resume__services-tour">
              <p>
                Пакетные туры
              </p>
            </div>
            <div class="resume__services-hotel">
              <p>
                Отели
              </p>
            </div>
          </div>
          <div class="resume__service-right">
            <div class="resume__service-number">
              <div class="resume__service-number-one">11</div>
              <div class="resume__service-number-two">2</div>
              <div class="resume__service-number-tree">2</div>
            </div>
          </div>
        </div>
        <div class="resume__serviec-all">
          <div class="resume__serviec-all-name">
            <p>
              Всего
            </p>
          </div>
          <div class="resume__servieces-all-numb">15</div>
        </div>
    </div>
</template>

<style>
.resume__services{
  width: 317px;
  margin-left: auto;
}
.resume__services-name {
  font-size: 13px;
  line-height: 15px;
  text-align: right;
  padding: 0 23px 7px 0;
}
.resume__services-scroll {
  border-top: 1px solid #c3c3c3;
  border-bottom: 1px solid #c3c3c3;
  padding: 15px 0;
  display: flex;
}
.resume__services-scroll p {
  font-size: 13px;
  line-height: 26px;
  padding: 3px 0 3px 6px;
}
.resume__service-right {
  display: flex;
  flex-direction: column;
  margin-left: 45px;
  font-weight: bold;
}
.resume__service-number {
  text-align: center;
  margin-top: 5px;
}
.resume__service-number-two {
  padding: 10px 0;
}
.resume__services-booking {
  width: 217px;
  border: 1px solid #B1E19B;
  background-color: #B1E19B;
  border-radius: 0 3px 3px 0;
}
.resume__services-tour {
  width: 54px;
  border: 1px solid #ACE2F8;
  background-color: #ACE2F8;
  border-radius: 0 3px 3px 0;
  margin: 2px 0;
}
.resume__services-tour  p{
  width: 92px;
  white-space: nowrap;
}
.resume__services-hotel {
  width: 36px;
  border: 1px solid #ACE2F8;
  background-color: #ACE2F8;
  border-radius: 0 3px 3px 0;
}
.resume__services-hotel p {
  width: 38px;
}
.resume__serviec-all {
  display: flex;
  justify-content: space-between;
  padding: 10px 40px 20px 6px;
}
.resume__serviec-all {
  font-weight: bold;
}
</style>