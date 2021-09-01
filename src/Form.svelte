<script>
import { text } from 'svelte/internal';

  import Input from './Input.svelte'
  let submitMessage = '<p>Submit</p>'
  const loginInputInfo = [
    {id: 1,
     type: 'text',
     icon: 'far fa-user',
     placeholder: 'Username: admin or User'
    },
    {
      id: 2,
      type: 'password',
      icon: 'fas fa-lock',
      placeholder: 'Password: ant.design',
    }
  ]
</script>

<form class="flex flex-col justify-center items-center mt-6">
  <button class="border-none m-2 text-xs">Account Login</button>
  
  {#each loginInputInfo as info, i}
    <Input type={info.type} icon={info.icon} placeholder={info.placeholder} />
  {/each}
  <div class="flex items-center m-2 w-60 justify-between" >
    <div class="flex justify-center items-center">
      <input type="checkbox">
      <p class="text-xs m-1">remember me</p>
    </div>
    <a class="text-xs" href="/">Forgot Password?</a>
  </div>
  <button class="bg-buttonColor text-white m-2 p-1 w-60">{@html submitMessage}</button>
</form>