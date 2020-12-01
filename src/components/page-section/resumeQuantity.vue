<template>
    <div class="resume__quantity">
        <div class="resume__quantity-left">
          <div class="resume__quantity-last-reviews">Последние отзывы</div>
          <a href="#">Все отзывы</a>
        </div>
        <div class="resume__quantity-right">
          <div class="resume__quantity-like">
            <img src="@/assets/img/reviews/like.svg" alt="like">
            <p>131</p>
          </div>
          <div class="resume__quantity-comment">
            <img src="@/assets/img/reviews/comment.svg" alt="comment">
            <p>14</p>
          </div>
        </div>
    </div>
</template>

<style>
.resume__quantity {
  display: flex;
  justify-content: space-between;
}
.resume__quantity-left {
  display: flex;
}
.resume__quantity-last-reviews {
  font-weight: bold;
  font-size: 16px;
  line-height: 16px;
  margin-right: 11px;
}
.resume__quantity-right {
  display: flex;
}
.resume__quantity-right img {
  padding-right: 3px;
}

.resume__quantity-like {
  display: flex;
  align-items: center;
}
.resume__quantity-comment {
  display: flex;
  align-items: center;
  margin-left: 16px;
}
</style>