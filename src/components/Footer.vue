<template>
  <footer>
      <section class="footer-top">
          <div class="wrap">
              <div class="menu-footer">
                  <div>
                      <h3>DC COMICS</h3>
                      <ul>
                          <li><a href="#">Characters</a></li>
                          <li><a href="#">Comics</a></li>
                          <li><a href="#">Movies</a></li>
                          <li><a href="#">TV</a></li>
                          <li><a href="#">Games</a></li>
                          <li><a href="#">Videos</a></li>
                          <li><a href="#">News</a></li>
                      </ul>
                      <h3>SHOP</h3>
                      <ul>
                          <li><a href="#">Shop DC</a></li>
                          <li><a href="#">Shop DC Collectibles</a></li>
                      </ul>
                  </div>
                  <div>
                      <h3>DC</h3>
                      <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                      </ul>
                  </div>
                  <div>
                      <h3>SITES</h3>
                      <ul>
                          <li><a href="#">DC</a></li>
                          <li><a href="#">MAD Magazine</a></li>
                          <li><a href="#">DC Kids</a></li>
                          <li><a href="#">DC Universe</a></li>
                          <li><a href="#">DC Power Visa</a></li>
                      </ul>
                  </div>
              </div>
          </div>
      </section>
      <section class="footer-bot">

          <div class="wrap">
              <button>SIGN-UP NOW!</button>
              <div>
                  <h2>FOLLOW US</h2>
                  <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                  <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                  <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
                  <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                  <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
              </div>
          </div>

      </section>
  </footer>
</template>

<script>
export default {
name:'Footer'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';

footer{
    .footer-top{
        height: 370px;
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
        overflow: hidden;
        .wrap{
            height: 100%;
            background-image: url('../assets/img/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: right;
            .menu-footer{
                display: flex;
                div{
                    padding-right: 2rem;
                }
                }
                h3{
                color:#fff;
                margin: 1rem 0;
                }
                a{
                display: inline-block;
                color: rgba(#fff, .4);
                font-size: 13px;
                margin-bottom: 0.50rem;
                &:hover{
                    color: #fff;
                 }
                }
        }
    }
    .footer-bot{
        padding: 30px 0;
        background-color: #303030;
        button{
            background: none;
            padding: 0.75rem;
            border: 2px solid $brand-blue;
            color: #fff;
            font-size: 15px;
            font-weight: 600;
            font-family: 'Roboto', sans-serif;
            cursor: pointer;
            &:hover{
                background-color: rgba(#fff, 0.2);
            }
            
        }
        div{
            display: flex;
            align-items: center;
            h2{
                color: $brand-blue;
            }
            img{
                margin-left: 1rem;
            }
        }
    }
}
</style>