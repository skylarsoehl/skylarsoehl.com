<template>
  <footer>
    <ul class="social-links">
      <a
        class="footer-link"
        href="https://drive.google.com/file/d/1RRNeEq6zwY_QaQvNHOqtpiWC640ZNlHr/view"
        >Résumé</a
      >
      <a class="footer-link" href="https://www.linkedin.com/in/skylarsoehl/"
        >LinkedIn</a
      >
      <a class="footer-link" href="https://www.instagram.com/skys.design/"
        >Instagram</a
      >
      <a class="footer-link" href="https://github.com/skylarsoehl">Github</a>
    </ul>
    <div class="footer-made-by">
      <p>Made with ♡ by Sky</p>
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style>
footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  background-color: #f83c22;
}

.social-links,
.footer-made-by {
  padding-left: 5.2vw;
  padding-right: 5.2vw;
}

.social-links > a {
  color: #efe7e0;
  text-decoration: none;
  margin-right: 34px;
  text-transform: uppercase;
}

.social-links > a:hover {
  transition: 800ms;
  color: black;
}

.footer-made-by {
  max-width: 300px;
  font-size: 14px;
  color: #efe7e0;
  font-weight: 500;
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: normal;
  font-size: 18px;
  line-height: 119.6%;
}
@media only screen and (max-width: 420px) {
  footer {
    flex-direction: column;
  }
  .social-links > a {
    margin-top: 10px;
    margin-left: 30px;
    margin-bottom: 10px;
    display: flex;
    justify-content: center;
  }
}
</style>
