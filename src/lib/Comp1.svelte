<script>
  export let app_function 
  // передается в этот компонент извне. Содержит функцию, которая будет вызвана в этом компоненте, при нажатии на кнопку.
  import Fa from 'svelte-fa'
  // отображения иконок Font Awesome
  import { faFlag } from '@fortawesome/free-solid-svg-icons'
  import { faGithub } from '@fortawesome/free-brands-svg-icons';
</script>

<div class='wrapper'>
   <!-- добавление иконок  -->
   <Fa icon={faFlag} />
   <Fa icon={faGithub} />
<h1>
  Component 1
  <!-- Заголовок 1 уровня --> 
</h1>
<div>
  <button on:click={()=>app_function('Сообщение от Comp1')}>Кнопка 1</button>
  <!-- Кнопка вызывает  функцию app_function  и передает сообщение-->
</div>
</div>

<style>
  button{
      width: 100px; 
      height:50px;
      background-color: purple;
      color:azure
  }
  .wrapper{
      border:1px solid silver;
      border-radius: 30px;
      padding:30px;
  }
</style>