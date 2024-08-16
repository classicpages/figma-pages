<template>
  <div class="section-two">
    <div class="section-content">
      <div class="free">Free Sample</div>
      <div class="ll">
        <h2 class="Powerful">Powerful Generator and Free Figma Sources</h2>
      </div>
      <div class="la">
        <p class="start">
          Startup Framework contains components and complex blocks which can
          easily be integrated into almost any design. All of the components are
          made in the same style, and can easily be integrated into projects,
          allowing you to create hundreds of solutions.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionTwo",
};
</script>

<style scoped>
.section-two {
  background-image: url("/public/Image.png");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  color: white;
  max-height: 540px;
  max-width: 100%;
  padding: 116px 0;
  background-color: #2f1893;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.ll {
  max-width: 815px;
  max-height: 140px;
}

.section-content {
  max-height: 307px;
}

.free {
  font-size: 19px;
  font-weight: 400;
}

.Powerful {
  font-size: 58px;
  font-weight: 600;
  max-height: 140;
}

.la {
  width: 775px;
  max-height: 84px;
  text-align: center;
}

.start {
  font-size: 18px;
  font-weight: 500px;
  line-height: 28px;
}
/* Responsive Styles */
@media (max-width: 480px) {
  .free {
    font-size: 14px;
  }

  .Powerful {
    font-size: 20px;
  }

  .start {
    font-size: 0.9rem;
  }
}

@media (min-width: 481px) and (max-width: 768px) {
  .free {
    font-size: 16px;
  }

  .Powerful {
    font-size: 25px;
  }

  .start {
    font-size: 1rem;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .free {
    font-size: 17px;
  }

  .Powerful {
    font-size: 35px;
  }

  .start {
    font-size: 1.1rem;
  }
}

@media (min-width: 1025px) and (max-width: 1200px) {
  .free {
    font-size: 18px;
  }

  .Powerful {
    font-size: 45px;
  }

  .start {
    font-size: 1.2rem;
  }
}

@media (min-width: 1201px) and (max-width: 1440px) {
  .free {
    font-size: 19px;
  }

  .Powerful {
    font-size: 50px;
  }

  .start {
    font-size: 1.3rem;
  }
}

@media (min-width: 1441px) {
  .free {
    font-size: 19px;
  }

  .Powerful {
    font-size: 58px;
  }

  .start {
    font-size: 1.5rem;
  }
}

</style>  