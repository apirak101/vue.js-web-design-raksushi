<template>
    <div class="header">
        <div class="logo-left">
            <div class="logo"><a href="#Home">rakSushi.</a></div>
        </div>
        <div class="menu-right">
            <ul>
                <li><a href="#Home">HOME</a></li>
                <li><a href="#ourstory">OUR STORY</a></li>
                <li><a href="#Menu">MENU</a></li>
                <li><a href="#contact">CONTACT</a></li>
            </ul>

            <div class="dropdown">
                <i class='fas fa-bars' style='font-size:30px; color:#fff;'></i>
                <div class="dropdown-content">
                    <a href="#Home">HOME</a>
                    <a href="#ourstory">OUR STORY</a>
                    <a href="#Menu">MENU</a>
                    <a href="#contact">CONTACT</a>
                </div>
            </div>
        </div>
    </div>

    
</template>

<script>
export default {
    name: 'H-Header'
}
</script>

<style>
.header {
    width: 100%;
    height: 13vh;
    background: var(--bg-color);
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.7);

    position: fixed;
    top: 0;
    z-index: 999;
}

.logo-left,
.menu-right {
    flex: 1;
}

ul {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    list-style: none;
    gap: 35px;
}

li a {
    font-family: var(--font-text);
    color: var(--text-color);
    font-size: 16px;
    cursor: pointer;
    text-decoration: none;
    transition: 300ms;
}

li a:hover {
    color: var(--color-orange);
}

.logo a {
    text-decoration: none;
    font-family: var(--font-logo);
    color: var(--text-color);
    font-size: 45px;
    cursor: pointer;
}


.dropdown {
    position: relative;
    display: none;
   
}


.dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
    z-index: 1;
}


.dropdown-content a {
    font-family: var(--font-text);
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
}


.dropdown-content a:hover {
    background-color: #ababab
}


.dropdown:hover .dropdown-content {
    display: block;
}


.dropdown:hover .dropbtn {
    background-color: #3e8e41;
}

.dropbtn {
    background-color: #4CAF50;
    color: white;
    padding: 16px;
    font-size: 16px;
    border: none;
    cursor: pointer;
    font-family: var(--font-text);
}



@media (max-width: 740px) {
    ul {
        display: none;
    }

    .dropdown {
        position: relative;
        display: inline-block;

    }
 .header{
    
    justify-content: left;
    gap: 1rem;
 }
    .logo-left,
    .menu-right {
        margin: 1rem;
        flex: 0;
}
}
</style>