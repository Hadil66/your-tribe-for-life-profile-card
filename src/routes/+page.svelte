


<script>
	export let data;
</script>

<main>
    <section>
        <div id="blueBorder1">        
            <div id="orangeBorder1"> </div>
    </div>
    </section>

    <article>
        <div>
            <h1>{data.person.name} {data.person.surname} </h1> 
            <div class="links">
            <a href="{data.person.website}">    
                <svg id="github" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 30 30">
                    <path d="M15 3C8.373 3 3 8.373 3 15c0 5.623 3.872 10.328 9.092 11.63a1.751 1.751 0 01-.092-.583v-2.051h-1.508c-.821 0-1.551-.353-1.905-1.009-.393-.729-.461-1.844-1.435-2.526-.289-.227-.069-.486.264-.451.615.174 1.125.596 1.605 1.222.478.627.703.769 1.596.769.433 0 1.081-.025 1.691-.121.328-.833.895-1.6 1.588-1.962-3.996-.411-5.903-2.399-5.903-5.098 0-1.162.495-2.286 1.336-3.233-.276-.94-.623-2.857.106-3.587 1.798 0 2.885 1.166 3.146 1.481A8.993 8.993 0 0115.495 9c1.036 0 2.024.174 2.922.483C18.675 9.17 19.763 8 21.565 8c.732.731.381 2.656.102 3.594.836.945 1.328 2.066 1.328 3.226 0 2.697-1.904 4.684-5.894 5.097C18.199 20.49 19 22.1 19 23.313v2.734c0 .104-.023.179-.035.268C23.641 24.676 27 20.236 27 15c0-6.627-5.373-12-12-12z"/>
                </svg> 
            </a>
            <a href="https://www.linkedin.com/in/hadil-ahmed-91b0252a3/">
                <svg id="linkedin" xmlns="http://www.w3.org/2000/svg" width="25" height="24">
                    <path d="M4.98 3.5C4.98 4.881 3.87 6 2.5 6S.02 4.881.02 3.5C.02 2.12 1.13 1 2.5 1s2.48 1.12 2.48 2.5zM5 8H0v16h5V8zm7.982 0H8.014v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0V24H24V13.869c0-7.88-8.922-7.593-11.018-3.714V8z"/>
                </svg>
            </a>
        </div>
        </div>
    </article>
    <section>
        <div id="blueBorder2"> 
            <div id="orangeBorder2"> </div>
        </div>
    </section>
</main>


<style>
    :root {
        /* theme 1 */
        --bg-clr: #fff4ec;
        --txt-clr: #020e16;
        --primary-clr-1: #e9631a;
        --primary-clr-2: #a9c2e0;

        background: var(--bg-clr);
    }

     @font-face {
            font-family: "Suse";
            src: url(src/routes/font/SUSE-Regular.ttf);
        }

     main {        
        font-family: "Suse";
    }

    #blueBorder1 {
        border: solid 0.5em var(--primary-clr-2);
        height: 2em;
        width: 2em;
    }

    #orangeBorder1 {
        border: solid 0.5em var(--primary-clr-1);
        height: 2em;
        width: 2em;
    }

    article {
        border: var(--primary-clr-1) solid 0.5em;
        padding: 1em;
        height: 12em;
        width: 25em;
        margin: 5em auto 10em auto;
    }

    div:first-child {
        border: var(--primary-clr-2) solid 0.5em;
        padding: 1em;
        height: 12em;
        width: 25em;
    }

    article:hover {
        animation: shake 1s ease-in-out ;
    }

    @keyframes shake {
        2% { transform: translateX(0); }
        10% { transform: translateX(-8px) rotate(-1deg); }
        20% { transform: translateX(10px) rotate(1deg); }
        30% { transform: translateX(-6px) rotate(-1deg); }
        40% { transform: translateX(8px) rotate(1deg); }
        50% { transform: translateX(-5px) rotate(0deg); }
        60% { transform: translateX(6px) rotate(1deg); }
        70% { transform: translateX(-4px) rotate(-1deg); }
        80% { transform: translateX(5px) rotate(1deg); }
        90% { transform: translateX(-3px) rotate(0deg); }
        100% { transform: translateX(0) rotate(0deg); }
    }

    h1 {
        text-align: end;
        padding: 0.8em;
    }

    svg:first-child {
        cursor: pointer;
        align-self: end;
     }

     svg:hover {
        scale: 1.5;
     }

     #github:hover {
        stroke: var(--primary-clr-1);
     }

     #linkedin:hover {
        stroke: var(--primary-clr-2);
     }

     .links {
        text-align: end;
        padding: 1.3em;
        gap: 0.5em;   
        display: flex;
        justify-content: flex-end;   
     }

     section:last-child {
        display: flex;
        justify-content: end;
     }

     #blueBorder2 {
        border: solid 0.5em var(--primary-clr-2);
        height: 2em;
        width: 2em;
    }

    #orangeBorder2  {
        border: solid 0.5em var(--primary-clr-1);
        height: 2em;
        width: 2em;
    }
</style>

