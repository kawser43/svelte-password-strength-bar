<script>
import PasswordStrength from "$lib/PasswordStrength.svelte";

let password = ""

</script>

<div class="w-72 mx-auto my-8">

    <div class="">
        <label for="password" class="block">Password</label>
        <input 
            class="w-full p-1 border border-gray-600 rounded"
            type="password" 
            placeholder="Password" 
            name="password"
            bind:value={password}
        />
    </div>
    
    <PasswordStrength {password}/>
</div>
