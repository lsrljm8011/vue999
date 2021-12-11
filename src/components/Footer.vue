<template>
  <footer id="footer">
    <div>
      <h4>email lsrljm98@gmail.com</h4>
      <p>
        <Link to="mailto:lsrljm98@gmail.com">lsrljm98@gmail.com</Link>
      </p>
    </div>
    <div>
      <h4>Kakao @serin8011</h4>
      <p><Link to="/">@serin8011</Link></p>
    </div>
    <div>
      <h4>social</h4>
      <ul>
        <li><a href="https://www.instagram.com/rnnsernn/">Instargram</a></li>
        <li><a href="https://lsrljm8011.github.io/dothome21/">Github</a></li>
        <li>
          <a href="https://lsrljm8011.github.io/dothome21/portfolio/index.html"
            >Portfolio</a
          >
        </li>
      </ul>
    </div>
  </footer>
</template>

<style lang="scss">
#footer {
  position: fixed;
  left: 0;
  bottom: 0;
  z-index: 1200;
  width: 100%;
  color: #fff;
  border-top: 1px solid #2e2e30;
  font-family: 'Rajdhani', 'Chosunilbo_myungjo';
  font-weight: 500;
  background: #000;
  display: flex;
  align-items: center;
  bottom: 0;

  div {
    text-align: center;
    padding: 30px;

    h4,
    p,
    ul {
      display: inline-block;
    }

    h4 {
      font-family: 'Rajdhani', 'Chosunilbo_myungjo';
      font-weight: 500;
      opacity: 0.6;
      padding: 0 10px;
    }
  }

  div:nth-child(1) {
    flex: 1 1 25%;
    border-right: 1px solid #2e2e30;
  }

  div:nth-child(2) {
    flex: 1 1 20%;
    border-right: 1px solid #2e2e30;
  }

  div:nth-child(3) {
    flex: 1 1 55%;

    li {
      display: inline-block;
      padding: 0 10px;
    }
  }
}
</style>
