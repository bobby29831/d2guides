<script>
    import "../app.css";
    import File from "$lib/File.svelte";
    import Folder from "$lib/Folder.svelte";
</script>

<div class="sm:hidden bg-yellow-200 flex items-center gap-5 justify-center p-5 rounded-md mx-5 mt-5 border-yellow-300 border-2">
    <i class="fa-solid fa-circle-exclamation text-yellow-500 scale-150"></i>
    <p class="text-black">
        Because you're on a small device, the website may not display content properly.
        Better mobile reactivity is coming soon.
    </p>
</div>

<nav class="flex justify-center">
    <ul class="menu menu-horizontal bg-base-200 rounded-box mt-10">
        <li>
            <a href="/">
                <i class="fa-solid fa-house"></i>
                <p>Home</p>
            </a>
        </li>
        <File text="About Us" href="/about"></File>
        <Folder text="Guides" href="/guides"></Folder>
        <li>
            <a href="https://github.com/bobooski/d2guides">
                <i class="fa-brands fa-github"></i>
                <p>Contribute</p>
            </a>
        </li>
    </ul>
</nav>

<slot />