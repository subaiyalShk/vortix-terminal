<script>
  import Typewriter from 'svelte-typewriter'
  let input ='';
  let messageThread = [
    {userName:'vortix', 'message':'welcome to tracerlabs'},
  ]
</script>

<main>
  <Typewriter cursor=true keepCursorOnFinish=true >
    <p>Hi welcome to TracerLabs. We are a web and mobile app development Agency. checkout our recent projects below </p>
  </Typewriter>
</main>

<style>
  line{
    display: flex;
  }
  p{
    transistion-delay: 1ms;
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
</style>
