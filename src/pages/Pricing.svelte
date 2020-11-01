<script>
  export const pricings = [
    {
      name: "Mobile Applications",
      sub: "₦78,000",
      lang: ["XML", "JAVA", "KOTLIN", "SWIFT", "DART"],
      id: 1,
      non: "",
    },
    {
      name: "Full Stack Development",
      sub: "₦45,000",
      lang: ["HTML", "CSS", "JavaScript", "MySQL", "PHP"],
      id: 2,
      non: "",
    },
    {
      name: "Front-End Development",
      sub: "₦35,000",
      lang: ["HTML", "CSS", "JavaScript", "MySQL", "PHP"],
      id: 3,
      non: "",
    },
    {
      name: "Digital Marketing",
      sub: "₦20,000",
      lang: ["SEO", "SEM", "HTML", "CSS", "JAVASCRIPT"],
      id: 4,
      non: "",
    },
  ];
</script>

<style>
  .section-title {
    text-align: center;
    padding-bottom: 30px;
  }
  h2 {
    font-size: 32px;
    font-weight: 600;
    text-transform: uppercase;
    margin-bottom: 20px;
    padding-bottom: 20px;
    position: relative;
    font-family: "Poppins", sans-serif;
    color: #dc143c;
  }
  .row {
    justify-content: center;
  }
  .box {
    padding: 40px;
    margin-bottom: 30px;
    margin-left: 0.5rem;
    margin-right: 0.5rem;
    box-shadow: 0px 0px 30px rgba(73, 78, 92, 0.15);
    background: #fff;
    text-align: center;
    position: relative;
  }
  h3 {
    font-weight: 300;
    margin-bottom: 15px;
    font-size: 20px;
  }
  h4 {
    font-size: 46px;
    color: crimson;
    font-weight: 400;
    font-family: "Open Sans", sans-serif;
    margin-bottom: 25px;
  }
  h4 span {
    color: #bababa;
    font-size: 18px;
    display: block;
  }
  ul li {
    padding: 12px 0;
    background: #fff;
    margin-bottom: 0.2rem;
    transform: skewY(3deg);
  }
  ul {
    padding: 0;
    list-style: none;
    color: #999;
    text-align: left;
    line-height: 20px;
    transform: skewY(-3deg);
    background: #dc143c;
  }
</style>

<section id="price" class="pricing section-bg">
  <div class="container">
    <div class="section-title">
      <h2 data-aos="fade-in" class="aos-init aos-animate">Pricing</h2>
      <p data-aos="fade-in" class="aos-init aos-animate">
        You can choose one from the tracks below
      </p>
    </div>

    <div class="row ">
      {#each pricings as pricing}
        <div class="col-lg-4 box">
          <h3>{pricing.name}</h3>
          <h4>{pricing.sub} <br /> <span>per month</span></h4>
          <ul>
            {#each pricing.lang as lang}
              <li>{lang}</li>
            {/each}
          </ul>
          <a href="#" class="btn btn-red mt-3">Get Started</a>
        </div>
      {/each}
    </div>
  </div>
</section>
