<template>
  <div class="resume__info">
    <div class="resume__photo">
      <img
        class="photo"
        src="@/assets/img/photo.png"
        alt="Photo"
      >
    </div>
    <div class="resume__namedesc">
      <div class="resume__name">
        <p class="resume__name-text">
          Вероника Ростова
        </p>
        <p class="resume__professional">
          Менеджер по продажам
        </p>
        <div class="resume__description-text">
          <p class="resume__description">
            Подберу для вас самые лучшие предложения.
            Мои услуги абсолютно бесплатны
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.resume__info {
  display: flex;
  position: relative;
}
.photo {
  border-radius: 50%;
  position: relative;
  z-index: 2;
}
.resume__namedesc {
  margin-left: 10px;
  height: 100px;
}
.resume__name {
  font-weight: bold;
  font-size: 16px;
  line-height: 20px;
}
.resume__professional {
  font-size: 12px;
  font-weight: normal;
  line-height: 20px;
  color: #808080;
  margin-top: 2px;
}
.resume__description-text {
  font-size: 14px;
  line-height: 20px;
  font-weight: normal;
  position: absolute;
  left: 90px;
}
.resume__description {
  max-width: 365px;
  background: #FFFBC8;
  border: 1px solid #DADADA;
  border-radius: 5px;
  padding: 10px 0 10px 40px;
  z-index: 1;
}
</style>