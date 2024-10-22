<script></script>

<template>
    <div class="contacts__block">
        <div class="contacts__item">
            <img src="../assets/img/location.png" alt="">
            <p>Город Москва</p>
        </div>
        <div class="contacts__item">
            <img src="../assets/img/phone-red.png" alt="">
            <p>+7 901 218-50-41</p>
        </div>
        <div class="contacts__item">
            <img src="../assets/img/email.png" alt="">
            <p>Moscow@moscow.ru</p>
        </div>
        <div class="contacts__item">
            <img src="../assets/img/clock.png" alt="">
            <p>
                Пн - Пт: 9:00 - 19:00 <br>
                Сб: 9:00 - 18:00 <br>
                Вс - выходной <br>
            </p>
        </div>
    </div>
    <button class="btn btn-red">Написать нам</button>
</template>


<style scoped lang="scss">

@mixin flex($fd, $jc, $ai){
    display: flex;
    flex-wrap: wrap;
    flex-direction: $fd;
    justify-content: $jc;
    align-items: $ai;
}

.contacts__block{
    width: 630px;
    margin: 60px auto;
    @include flex(row, space-between, center);
    .contacts__item{
        @include flex(row, left, center);
        margin-bottom: 50px;
        margin-right: 5px;
        p{
            margin-left: 15px;
        }
    }
    .contacts__item:last-child{
        margin-right: 0;
    }
}
.btn-red{
    @include flex(row, center, center);
    color: #FFF;
    font-size: 16px;
    font-weight: 500;
}

</style>