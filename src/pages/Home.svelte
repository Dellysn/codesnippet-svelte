<script>
  import Carousel from "@beyonk/svelte-carousel";
  import { ChevronLeftIcon, ChevronRightIcon } from "svelte-feather-icons";
</script>

<style>
  .control :global(svg) {
    width: 100%;
    height: 100%;
    color: #fff;
    border: 2px solid #fff;
    border-radius: 32px;
  }
  img {
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    height: 100%;
  }
  .slide-content {
    position: relative;
  }
  .carousel-text {
    position: absolute;
    bottom: 0%;
    left: 0%;
    z-index: 999.99;
    width: 50%;
    display: flex;
    flex-direction: column;
    color: #f0f0f0;
    background-color: rgba(220, 20, 60, 0.829);
    padding: 1rem;
  }
  @media (max-width: 768px) {
    h2 {
      font-size: 1rem;
    }
    p {
      font-size: 0.67rem;
    }
    .carousel-text {
      width: 100%;
    }
    .slide-content {
      height: 48vh;
    }
  }
</style>

<div class="carousel-space">
  <Carousel perPage={1} easing="ease-out" loop={true} autoplay={4000}>
    <span class="control" slot="left-control">
      <ChevronLeftIcon />
    </span>
    <div class="slide-content">
      <!-- svelte-ignore a11y-img-redundant-alt -->
      <img src="images/ca-1.jpg" alt="Carousel Image" />
      <div class="carousel-text">
        <h2>Welcome To Code Snippet!</h2>
        <p>
          We are a software startup in the first year of our operations. Our
          founders are entrepreneurs and Software Engineers with many years of
          of experience in Information and Communication Technology
        </p>
      </div>
    </div>
    <div class="slide-content">
      <!-- svelte-ignore a11y-img-redundant-alt -->
      <img src="images/ca-2.jpg" alt="Carousel Image" />
      <div class="carousel-text">
        <h2>Welcome To Code Snippet!</h2>
        <p>We are here offer some of the best coding courses.</p>
      </div>
    </div>
    <div class="slide-content">
      <!-- svelte-ignore a11y-img-redundant-alt -->
      <img src="images/ca-3.png" alt="Carousel Image" />

      <div class="carousel-text">
        <h2>Welcome To Code Snippet!</h2>
        <p>
          We are out to offer quality software solutions and training is many
          technologies and software stacks.
        </p>
      </div>
    </div>

    <span class="control" slot="right-control">
      <ChevronRightIcon />
    </span>
  </Carousel>
</div>
