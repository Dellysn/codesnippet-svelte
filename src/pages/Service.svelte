<script>
  export const services = [
    {
      title: "Web Development",
      icon: "",
      image: "images/serv-1.jpg",
      content:
        "We build custom web application using modern programming techniques and methodologies. We analyze the business or brief, then provide an appropriate solution. For developer who wishes to advance his skills to world class level, Your seat is reserved @ Code Snippet",
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
    {
      title: "Full Stack Development",
      icon: "",
      image: "images/serv-2.jpg",
      content:
        "Code Snippet Design combines web design, usability (ease of use), search engine optimization for high rankings, and marketing knowhow into each website we build. It's better, faster and cheaper to do it all at once than to bring new companies into the mix after the fact. Our market-savvy website design team can not only design a custom website design that represents you well, but can also increase your exposure on the Internet and help to attract customers and increase your sales.",
      id: 4,
    },
  ];
  import { fade } from "svelte/transition";
</script>

<style>
  .card {
    border: 0;
    padding: 0 30px;
    margin-bottom: 60px;
    position: relative;
    background: #0000;
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    /* background-color: #fff;
    background-clip: border-box;
    border: 1px solid #00000020; */
    border-radius: 0.25rem;
  }
  .card-title a {
    text-decoration: none;
    color: #ed143d;
    letter-spacing: 5px;
    font-weight: 700;
  }
  .card-body {
    z-index: 10;
    background: #fff;
    border-top: 4px solid crimson;
    padding: 30px;
    box-shadow: 0px 2px 15px rgba(0, 0, 0, 0.1);
    margin-top: -60px;
    transition: 0.3s;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .card-img {
    width: calc(100% + 60px);
    margin-left: -30px;
    overflow: hidden;
    z-index: 9;
    border-radius: 0;
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
    text-align: center;
  }
</style>

<section id="services" in:fade>
  <div class="container">
    <h2 class="heading-2">Service</h2>
    <div class="row">
      {#each services as service}
        <div
          class="col-md-6 d-flex  aos-init aos-animate"
          data-aos="fade-right">
          <div class="card">
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <div class="card-img"><img src={service.image} alt="Photo" /></div>

            <div class="card-body">
              <!-- svelte-ignore a11y-invalid-attribute -->
              <h5 class="card-title"><a href="#">{service.title}</a></h5>
              <p class="card-text">{service.content}</p>
              <div class="read-more">
                <!-- svelte-ignore a11y-invalid-attribute -->
                <a href="#" class="btn btn-red"><i
                    class="icofont-arrow-right" />
                  Read More</a>
              </div>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
