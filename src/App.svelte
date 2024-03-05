<script>
  import Typewriter from 'svelte-typewriter'
  let input ='';
  let messageThread = [
    {userName:'vortix', 'message':'welcome to tracerlabs'},
  ]
</script>

<main>
  <div class=fakeMenu>
    <div class="fakeButtons fakeClose"></div>
    <div class="fakeButtons fakeMinimize"></div>
    <div class="fakeButtons fakeZoom"></div>
  </div>
  <div class="fakeScreen">
    <div class="message-line">
      <p>
        subaiyalshk@tracerlabs.io:
        <Typewriter interval={30} element="div" --cursor-color="#00FF00" cursor={true} keepCursorOnFinish={true} mode="cascade">
          Welcome to TracerLabs. Since 2016 we have been building digital products and solutions as web and mobile apps. Our expertise has enabled us help numerous business with Cyber Security, Planning, Prototyping, Development, Testing and Beyond. Check out some of our past projects and if you have any questions CLICK ON THE RED BUTTON.
        </Typewriter>
      </p>
    </div>
  </div>
</main>

<style>
  
  main{
    height:100vh;
  }

  #terminal-input{
    background-color: black;
    border-color: green;
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100vw;
    height: 20px;
    color: green;
  }

  #terminal-input:focus{
    border: 3px solid #555;
  }

  .fakeButtons {
    height: 10px;
    width: 10px;
    border-radius: 50%;
    border: 1px solid #000;
    position: relative;
    top: 6px;
    left: 6px;
    background-color: #ff3b47;
    border-color: #9d252b;
    display: inline-block;
  }

  .fakeMinimize {
    left: 11px;
    background-color: #ffc100;
    border-color: #9d802c;
  }

  .fakeZoom {
    left: 16px;
    background-color: #00d742;
    border-color: #049931;
  }

  .fakeMenu {
    position: fixed;
    width: 100vw;
    box-sizing: border-box;
    height: 40px;
    background-color: #bbb;
    margin: 0 auto;
    border-top-right-radius: 5px;
    border-top-left-radius: 5px;
  }

  .fakeScreen {
    background-color: #151515;
    box-sizing: border-box;
    width: 100vw;
    height: 100%;
    max-height: 100%;
    overflow: scroll;
    margin: 0 auto;
    padding: 20px;
    padding-top: 60px;
    border-bottom-left-radius: 5px;
    border-bottom-right-radius: 5px;
  }

  .message-line{
    display:flex;
  }

  .message-line p{
    color: white;
    font-size: 0.75rem;
  }

</style>
