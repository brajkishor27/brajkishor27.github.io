<template>
  <div>
    <rainbow-text text="Contact"></rainbow-text>
    <div class="links">
      <a href="https://twitter.com/braj_kishor97" class="social-link" title="Twitter"><i class="fa fa-twitter blue" aria-hidden="true"></i></a>
      <a href="https://dev.to/aspittel" class="social-link dev-to">
        <img src="https://d2fltix0v2e0sb.cloudfront.net/dev-badge.svg" alt="Ali Spittel's DEV Profile" class="dev-to-img"/>
      </a>
      <a href="https://github.com/brajkishor27.github.io" class="social-link" title="Github"><i class="fa fa-github purple" aria-hidden="true"></i></a>
      <a href="https://www.linkedin.com/in/braj-kishor-230334152/" class="social-link" title="Linkedin"><i class="fa fa-linkedin dark-blue" aria-hidden="true"></i></a>
      <a href="mailto:kumarbrajkishor96@gmail.com" class="social-link" title="email me"><i class="fa fa-envelope red" aria-hidden="true"></i></a>
      <a href="https://medium.com/on-learning-new-things" class="social-link" title="Medium"><i class="fa fa-medium green" aria-hidden="true"></i></a>
    </div>
  </div>
</template>

<script>
import RainbowText from "@/components/RainbowText"

export default {
  components: {
    'rainbow-text': RainbowText,
  } 
}
</script>

<style lang="scss" scoped>
.links {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
  -ms-flex-direction: row;
  flex-direction: row;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 100px;
  text-align: center;
  margin-bottom: 100px;
  flex-wrap: wrap;

  @media (max-width: 400px) {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
}

.social-link {
  font-size: 100px;
  
  @media (max-width: 700px) {
    font-size: 50px;
  }
}

.dev-to {
  margin-top: 5px;
}

.dev-to-img {
  height: 85px;
  width: 85px;

  @media (max-width: 700px) {
    height: 45px;
    width: 45px;
  }
}
.social-link:hover {
  opacity: .5;
}

.red {
  color: #ef5350;
}

.purple {
  color: #ab47bc;
}

.bright-blue {
  color: #651fff;
}

.dark-blue {
  color: #3949ab;
}

.blue {
  color: #2196f3;
}

.teal {
  color: #00bcd4;
}

.green {
  color: #4caf50;
}

.yellow {
  color: #ffc107;
}

.pink {
  color: #ff80ab;
}

.orange {
  color: #ff8f00;
}
</style>

