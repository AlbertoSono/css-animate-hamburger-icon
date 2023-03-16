# css-animate-hamburger-icon
Hamburger icon animeted with CSS3 only, no js 

\# based on: https://codepen.io/eduardoboucas/pen/rayExg


```
/* albertosono
css-animate-hamburger-icon
https://github.com/AlbertoSono/css-animate-hamburger-icon
*/
<style>
.burger {
   
  display: inline-block;
  border: 0;
  outline: 0;
  padding: 0;
  cursor: pointer;
  border-bottom: 4px solid currentColor;
  width: 28px;
  transition: border-bottom 1s ease-in-out;
  -webkit-transition: border-bottom 1s ease-in-out;
  border-radius: 20%;
  
}
.burger::-moz-focus-inner {
  border: 0;
  padding: 0;
}
.burger:before, .burger:after {
  content: "";
  display: block;
  border-bottom: 4px solid currentColor;
  width: 100%;
  margin-bottom: 5px;
  transition: transform 0.5s ease-in-out;
  -webkit-transition: -webkit-transform 0.5s ease-in-out;
  border-radius: 30%;
}
.burger-check {
  display: none;
}
.burger-check:checked ~ .burger {
  border-bottom: 4px solid transparent;
  transition: border-bottom 0.8s ease-in-out;
  -webkit-transition: border-bottom 0.8s ease-in-out;
}
.burger-check:checked ~ .burger:before, .burger-check:checked ~ .burger:after {
    transition: transform 0.5s ease-in-out;
  -webkit-transition: -webkit-transform 0.5s ease-in-out;
}
.burger-check:checked ~ .burger:before {
  -ms-transform: rotate(-405deg) translateY(6px) translateX(-6px);
      transform: rotate(-405deg) translateY(6px) translateX(-6px);
  -webkit-transform: rotate(-405deg) translateY(6px) translateX(-6px);
}
.burger-check:checked ~ .burger:after {
  -ms-transform: rotate(405deg) translateY(0) translateX(0);
      transform: rotate(405deg) translateY(0) translateX(0);
  -webkit-transform: rotate(405deg) translateY(0) translateX(0);
}
.burger-check:checked ~ .navigation {
  max-height: 500px;
  -webkit-transition: max-height 0.5s ease-in-out;
          transition: max-height 0.5s ease-in-out;
}
</style>
<input class="burger-check" id="burger-check" type="checkbox"><label for="burger-check" class="burger"></label>

```
