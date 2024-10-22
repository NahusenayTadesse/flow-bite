<div>
		<a href="/services" class="project">Services</a>
        <a href="/contact" class="contact">Contact Me</a>
</div>

<style>
    div {
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
        width: 100%;

    }
     .project, .contact:hover{
      
        background-color: var(--color-theme-1);
        color: white;
        text-decoration: none;
        width: 100px;
        padding: 10px;
        border: solid 1px;
        text-align: center;
        border-radius: 8px;
    }
    .contact, .project:hover {
        background-color: transparent;
        color: black;
        text-decoration: none;
        width: 100px;
        text-align: center;
        border: solid 1px;
        padding: 10px;
        border-radius: 8px;

    }
    a{
        width: 100%;
    }
</style>