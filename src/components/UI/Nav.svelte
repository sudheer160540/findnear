<script>
  //export let segment;
  
</script>

<style lang="scss">
  @import "./../theme.scss";

  nav {
    border-bottom: 1px solid rgba(255, 62, 0, 0.1);
    font-weight: 300;
    padding: 0 1em;
  }

  ul {
    margin: 0;
    padding: 0;
  }

  /* clearfix */
  ul::after {
    content: "";
    display: block;
    clear: both;
  }

  li {
    display: block;
    float: left;
  }

  [aria-current] {
    position: relative;
    display: inline-block;
  }

 

  a {
    text-decoration: none;
    padding: 1em 0.5em;
    display: block;
  }
  .header {
    width: 100%;
    height: 68px;
    background: #fff;
    margin-right: auto;
    margin-left: auto;
    padding-left: 24px;
    padding-right: 24px;
    position: fixed;
    z-index: 1007;
    box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.15);
  }
  .login {
    display: flex;
    padding: 0px 12.5rem;
    padding-top: 16px;
    img {
      width: 16px;
      height: 25px;
      margin-right: 1rem;
    }
  }
</style>

<!-- <nav class="header">

  <div class="row">
  
    <div class="col-sm-3">
      <a href="/">
        <img
          src="https://static.cure.fit/assets/images/curefit-v-man.svg"
          class="css-pszboc-headerLogo" />
      </a>
    </div>
    <div class="col-sm-6" />
    <div class="col-sm-3">

      <div class="login">
        <img src="https://static.cure.fit/assets/images/user-image.svg" />
        <span class="login-text">Login</span>
      </div>
    </div>

  </div>

</nav> -->
 <nav class="navbar navbar-expand-lg fixed-top shadow navbar-light bg-white">
        <div class="container-fluid">
          <div class="d-flex align-items-center"><a class="navbar-brand py-1" href="index.html"><img src="https://d19m59y37dris4.cloudfront.net/directory/1-5/img/logo.svg" alt="Directory logo"></a>
           
          </div>
          <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation"><i class="fa fa-bars"></i></button>
          <!-- Navbar Collapse -->
          <div class="collapse navbar-collapse" id="navbarCollapse">
           
            <ul class="navbar-nav ml-auto">
              <li class="nav-item dropdown"><a class="nav-link dropdown-toggle active" id="homeDropdownMenuLink" href="index.html" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                   Home</a>
                <div class="dropdown-menu" aria-labelledby="homeDropdownMenuLink"><a class="dropdown-item" href="index.html">Rooms</a><a class="dropdown-item" href="index-2.html">Restaurants</a><a class="dropdown-item" href="index-3.html">Travel</a><a class="dropdown-item" href="index-4.html">Real Estate <span class="badge badge-info-light ml-1 mt-n1">New</span></a></div>
              </li>
           
              <!-- /Megamenu end-->
          
            
              <li class="nav-item"><a class="nav-link" href="login.html">Sign in</a></li>
              <li class="nav-item"><a class="nav-link" href="signup.html">Sign up</a></li>
            </ul>
          </div>
        </div>
      </nav>