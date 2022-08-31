<template>
    <footer class="footer">
        <div class="footer-wrapper">
    <div class="rectangle"></div>
    <div class="links">
        
        <div class="link">
            <h2 class="link-title">
    Для связи
            </h2>
            <p class="phone">
                <img src="../assets/images/SocialIcons.png" alt="" class="img-phone">
    7 (926) 126 64-57
            </p>
            <p class="phone">
                <img src="../assets/images/SocialIcons2.png" alt="" class="img-phone">
                7 (926) 126 64-57   
            </p>
            <p class="phone">
                <img src="../assets/images/SocialIcons3.png" alt="" class="img-phone">
                7 (926) 126 64-57   
            </p>
        </div>
    
        <div class="link">
    <h2 class="link-title2">
        Компания
    </h2>
        <p class="usl">
    Услуги
        </p>
        <p class="usl">
    Кейсы
        </p>
        <p class="usl">
    Контакты
        </p>
        <p class="usl">
    Сотрудничество
        </p>
    
        </div>
        <div class="link">
            <h2 class="link-title2">
                Документы
            </h2>
                <p class="usl">
            Политика конфиденциальности
                </p>
                <p class="usl">
            Пользовательское соглашение
                </p>
        </div>
        <div class="link">
            <h2 class="link-title2">
                Будьте в курсе
            </h2>
            <div class="e-mail-input">
    <input type="email" value="E-mail" class="email" >
    
    </div>
    <div class="soc">
    <img src="../assets/images/insta.png" alt="" class="soclink">
    <img src="../assets/images/VK.png" alt="" class="soclink">
    <img src="../assets/images/FB.png" alt="" class="soclink">
    </div>
        </div>
        </div>
    </div>
    
    <div class="author">
        Copyright © 2022 SCID
    </div>
    
    </footer>

</template>

<script>


</script>

<style scoped>

    .footer{
        background-color: #00A76B;
        max-width: 1440px;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        height: 366px;
    
    }
    
    .footer-wrapper{
        max-width: 1440px;
        display: flex;
        flex-direction: row;
        align-items: center;
        height: 186px;
        margin-top: 76px;
        justify-content: center;
        
    }
    
    
    .rectangle{
        width: 108px;
        height: 154px;
        border-radius: 16px;
        background: #009B63;
        margin-left: 80px ;
        
    }
    
    .links{
        
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-gap: 90px;
    margin-left: 80px;
    margin-right: 80px;
    max-width: 1280px;
    }
    
    .link{
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;
    }
    
    .link-title{
        font-family: sans-serif;
        font-weight: 600;
        font-size: 20px;
        font-style: normal;
        line-height: 30px;
        color: #fff;
        margin-bottom: 30px;
    }
    
    
    .phone{
        font-family: sans-serif;
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        line-height: 20px;
        color: #fff;
        margin-bottom: 20px;
    }
    
    .img-phone{
        margin-right: 8px;
        width: 32px;
        height: 32px;
    }
    
    .usl{
        font-family: sans-serif;
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 130%;
        margin-bottom: 16px;
        color: #fff;
    }
    
    .link-title2{
        font-family: sans-serif;
        font-weight: 600;
        font-size: 20px;
        font-style: normal;
        line-height: 30px;
        color: #fff;
        margin-bottom: 34px;
    }
    
    .email{
        
        color: #fff;
        font-family: sans-serif;
        font-size: 14px;
        font-weight: 400;
        line-height: 24px;
        border: 0;
       padding-right: 4.71%;
        height: 40px;
        width: 255px;
        padding-left: 4.71%;
        background: url(../assets/images/send.png)no-repeat right;
        margin-right: 11px;
    }
    
    .e-mail-input{
        background-color: #00BB78;
         border-radius: 10px;
    }
    
    .soc{
        display: flex;
        flex-direction: row;
        align-items: flex-start;
        margin-top: 50px;
    }
    
    .soclink{
        margin-left: 16px;
    }
    
    .soclink:first-child{
        margin-left: 0;
    }
            
    .author{
        display: flex;
        flex-direction: row;
    align-items: center;
    justify-content: center;
    color: #fff;
        font-size: 16px;
        font-weight: 400;
        font-family: sans-serif;
        margin: 76px auto 26px auto;
        
    }
</style>