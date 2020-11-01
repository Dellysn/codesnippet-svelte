<script>
  import Carousel from "@beyonk/svelte-carousel";
  import { ChevronLeftIcon, ChevronRightIcon } from "svelte-feather-icons";
  export const testimonials = [
    {
      title: "Web Development",
      icon: "",
      image: "images/serv-1.jpg",
      content:
        "We build custom web application using modern programming techniques and methodologies. We analyze the business or brief, then provide an appropriate solution.",
      id: 1,
    },

    {
      title: "Mobile Development",
      icon: "",
      image: "images/serv-3.jpg",
      content:
        "To the success of your business accross different industries, We offer full-scale Mobile Apps for mobile users which will contribute to the growth of your business and capture targerted users.",
      id: 2,
    },
    {
      title: "Digital Marketing",
      icon: "",
      image: "images/serv-4.jpg",
      content:
        "Getting your social media presence to generate leads and more revenue, code snippet will get you on track with live time results!, We excel in Facebook, Instagram, Twitter, LinkedIn etc.",
      id: 3,
    },
  ];
</script>

<style>
  .box {
    /* padding: 40px; */
    margin-bottom: 30px;
    margin-left: 0.5rem;
    margin-right: 0.5rem;
    box-shadow: 0px 0px 30px rgba(73, 78, 92, 0.15);
    background: #fff;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .section-title {
    text-align: center;
    /* padding-bottom: 30px; */
  }
  h2 {
    font-size: 32px;
    font-weight: 600;
    text-transform: uppercase;
    margin-bottom: 20px;
    padding-bottom: 20px;
    position: relative;
    font-family: "Poppins", sans-serif;
    color: #fff;
  }
  section {
    background-color: #dc143ce0;
    transform: skewY(-6deg);
    padding: 8rem 0;
    margin-bottom: 3rem;
  }
  .container {
    transform: skewY(6deg);
  }
</style>

<section id="testimonial" class="section-title">
  <div class="container">
    <h2>Testimonials</h2>
    <Carousel
      perPage={{ 800: 3, 500: 2 }}
      easing="ease-out"
      dots={false}
      loop={true}
      autoplay={4000}>
      {#each testimonials as testimonial}
        <div class="slide-content">
          <div class="card box">
            <img src="images/serv-1.jpg" class="card-img-top" alt="..." />
            <div class="card-body">
              <p class="card-text">{testimonial.content}</p>
            </div>
          </div>
        </div>
      {/each}
    </Carousel>
  </div>
</section>
