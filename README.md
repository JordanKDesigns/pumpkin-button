# Pumpkin CTA Button

### HTML

     <a href="#">
     <div class="pumpkin-btn" tabindex="0" role="button">
       <div class="pumpkin-shape"> <span class="pumpkin-face"></span>
         <div class="pumpkin-bar">Signup Now</div>
       </div>
     </div>
     </a>
     
### CSS

      /* Pumpkin Button with Vendor Prefixes */
      /* -----------------*/

      /* Container for Pumpkin Button */
      .pumpkin-btn {
        cursor: pointer;
        text-align: center;
        margin: 0 auto;
        width: 100%;
        max-width: 285px;
        -webkit-transition: all 0.3s ease-in-out;
        -o-transition: all 0.3s ease-in-out;
        transition: all 0.3s ease-in-out;
      }

      /* Button raise up on hover */
      .pumpkin-btn:hover {
        -webkit-transform: translateY(-4px);
            -ms-transform: translateY(-4px);
                transform: translateY(-4px);
      }

      /* Pumpkin Front Shape */
      .pumpkin-shape {
        width: 90px;
        height: 100px;
        border-radius: 50%;
        background-color: #ff8f00;
        position: relative;
        border: 1px solid rgba(147, 55, 0, 0.2);
      }

      /* Pumpkin Back Shape */
      .pumpkin-shape::before {
        content: "";
        display: block;
        width: 120px;
        height: 100px;
        border-radius: 50%;
        position: relative;
        z-index: -2;
        left: -16px;
        background: -webkit-gradient(linear, left top, right top, from(rgba(255, 155, 50, 1)), color-stop(40%, rgba(255, 155, 50, 1)), color-stop(60%, rgba(240, 100, 0, 1)), to(rgba(240, 100, 0, 1)));
        background: -o-linear-gradient(left, rgba(255, 155, 50, 1) 0%, rgba(255, 155, 50, 1) 40%, rgba(240, 100, 0, 1) 60%, rgba(240, 100, 0, 1) 100%);
        background: linear-gradient(90deg, rgba(255, 155, 50, 1) 0%, rgba(255, 155, 50, 1) 40%, rgba(240, 100, 0, 1) 60%, rgba(240, 100, 0, 1) 100%);
      }

      /* Pumpkin Stem */
      .pumpkin-shape::after {
        content: "";
        border-left: 45px solid #0AA510;
        border-top: 45px solid transparent;
        position: absolute;
        top: -16px;
        left: 34px;
        -webkit-transform: rotate(22deg);
            -ms-transform: rotate(22deg);
                transform: rotate(22deg);
        z-index: -3;
      }

      /* Button Bar with Text */
      .pumpkin-bar {
        width: 210px;
        height: 60px;
        border-radius: 0 10px 10px 0;
        background-color: #000;
        position: absolute;
        bottom: 15px;
        left: 90px;
        z-index: -4;
        padding: 10px;
        font-size: 22px;
        font-weight: bold;
        color: #fff;
      }
      
### Face Image

![Pumpkin Face](pumpkin-face.png)

### Face CSS

      /* Pumpkin Face */
      .pumpkin-face {
        background-image: url('');
        background-repeat: no-repeat;
        width: 90px;
        height: 100px;
        position: absolute;
        top: 52%;
        left: 52%;
        -webkit-transform: translate(-50%, -50%);
            -ms-transform: translate(-50%, -50%);
                transform: translate(-50%, -50%);
        -webkit-transition-property: -webkit-filter;
        transition-property: -webkit-filter;
        -o-transition-property: filter;
        transition-property: filter;
        transition-property: filter, -webkit-filter;
        -webkit-transition-duration: 0.3s;
             -o-transition-duration: 0.3s;
                transition-duration: 0.3s;
      }

      /* Pumpkin Face Light on Hover */
      .pumpkin-btn:hover .pumpkin-face {
        -webkit-filter: brightness(12);
                filter: brightness(12);
      }
