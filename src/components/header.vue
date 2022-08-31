<template>
    <header class="header">
        <div class="wrapper">
           <div class="header__wrapper">
               <div class="header__logo">
                   <a href="index.html" class="headerlogo_link">
                       <img src="../assets/images/logo.jpg" alt="logo" class="headerlogo-pic">
                   </a>
                   
                           </div>
                   
                      <nav class="header__nav">
                           <ul class="header__list">
                           <li class="header__item">
                                 <a href="#" class="header__link">КЕЙСЫ
                          </a>
                           </li>
                           <li class="header__item">
                               <div class="img_header">
                               <img src="../assets/images/Union.png" alt="" class="union_img">
                      <a href="#" class="header__link">БИЗНЕСУ</a></div>
                       </li>
                         <li class="header__item">
                                 <a href="#" class="header__link">УСЛУГИ</a>
                       </li>
                          <li class="header__item"> 
                              <a href="#" class="header__link">КОНТАКТЫ</a>
                       </li>
                               </ul>
                               <input type="button" value="Заказать звонок" class="header__button">
                           </nav>
           </div>
        </div>
       </header>
</template>

<script>

</script>

<style scoped>
    .wrapper{
        max-width: 1280px;
        margin: 0 auto;
        
    }
    .header{
        position: static;
        top: 0;
        left: 0;
        width: 100%;
        
        box-shadow: 0px 4px 21px rgba(0,0,0,0.07);
        padding: 24px 80px;
        }

        .header__wrapper{
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content:space-between;
        flex-direction: row;
        }
        .header__logo{
            vertical-align: middle;
        }
        .header__nav{
        display: flex;
        flex-direction: row;
        align-items: center;
        
        
        }
        .header__list{
            display: flex;
            flex-wrap: wrap;
            list-style-type: none;
        }
        
        .header__item{
            margin-right: 48px;
            flex-direction: row;
        
        }
        .header__item:first-child{
            margin-right: 69px;
        }
        .img_header{
        display: flex;
        flex-direction: row;
        align-items: center;
        
        }
        .union_img{
            margin-right: 8px;
        }
        
        .header__button{
            display: flex;
            flex-direction: row;
        align-items: center;
        background-color: #fff;
            font-size: 16px;
            font-weight: 400;
            border-radius: 30px;
            border: 1.5px solid #00BB78;
            cursor: pointer;
            padding: 12px 28px;
            color: #00BB78;
            line-height: 22px;
            
        }
        
        .header__link{
            line-height: 22px;
            font-size: 16px;
            color: #0E0E0F;
            text-decoration: none;
            
        }
        
        .header__button:hover{
            background-color: #00BB78;
            color: #fff;
        }
        
        .header__link:hover, .header__link:focus, .header__link:active{
            color: #00BB78;
        }
</style>