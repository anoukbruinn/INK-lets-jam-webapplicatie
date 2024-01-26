<script>
    import { base } from '$app/paths';
	// export let data;
</script>

<section class="ourValues">

    <h1 class="title"> 
        <span style=" color: white;">Our</span> 
        <span style=" color: var(--Blue-Secondary);">Values</span> 
        <img class="morale" src="{base}/assets/Morale.png" alt="morale"> 
    </h1>
    <div class="values">
        <div class="values1"> 
            <h4>  
                <img src="{base}/assets/Checkbox.png" alt=""> 
                Respect 
            </h4>
            <h4>  
                <img src="{base}/assets/Checkbox.png" alt=""> 
                Protect
            </h4>
            <h4>  
                <img src="{base}/assets/Checkbox.png" alt=""> 
                Humanity 
            </h4>
        </div>
        <div class="values2"> 
            <h4>  
                <img src="{base}/assets/Checkbox.png" alt="">
                Transparency 
            </h4>
            <h4>  
                <img src="{base}/assets/Checkbox.png" alt=""> 
                Fairness
            </h4>
            <h4>  
                <img src="{base}/assets/Checkbox.png" alt=""> 
                Equality
            </h4>
        </div>
    </div>

    <div class="paragraphIntro"> 
        <div class="line2">  
            <img class= "line" src="{base}/assets/Line-blue.png" alt="line"> 
        </div>
        <div class="paragraph"> 
            <p class="introParagraph1"> 
                At INK, we believe that these values are the 
                foundation of a just and equitable society. 
            </p>
            <p class="introParagraph2">  
                We are committed to upholding these values in all of our work, 
                including our programs, our partnerships, and our interactions 
                with our stakeholders.
            </p>
        </div>
    </div>
</section>

<style>

    h1 {
        font-size: 50px;
        float: center;
        padding-top: 1em;
        display: flex;
        justify-content: center;
    }

    .values {
        display: flex;
        justify-content: center;
        padding: 1em;
    }

    h4 {
        font-family: var(--JubilatMedium-Roman);
        padding: 1em;
        align-content: center;
        font-size: 1.1em;
    }

    .ourValues {
        background-image: url(/assets/Group-1.png);
        height: 1000px;
        display: flex;
        align-items: center;
        flex-direction: column;

    }

    .paragraphIntro {
        display: flex;
        justify-content: center;
        padding: 2em;
    }

    .paragraph {
        padding-left: 1em;
    }

    .introParagraph1 {
        margin-bottom: 1em;
    }

    .introParagraph2 {
        margin-top: 1em;
    }

    .line2 {
        margin-top: 10px; 
    } 

    p {
        font-family: var(--Paragraph-Font);
    }

    
    @media (min-width: 48em) {

        .ourValues{
            background-image: url(/assets/Group-84.svg);
            padding-left: 10em;
            padding-right: 10em;
            padding-bottom: 5em;
            
        }

        .values {
            padding: 0;
            justify-content: center;
        }

        p {
            font-size: 20px;
            width: 30em;
        }

        h4 {
            font-size: 30px;
            width: 300px;
        }

        .paragraph {
            
            padding-top: 1em;
           
        }

        .line {
            height: 155px;
            padding-bottom: 10px;
        }

        .paragraphIntro {
            padding-bottom: 8em;
        }

        h1 {
            font-size: 80px;
            display: flex;
            justify-content: center;
        }

        .morale {
            width: 79px;
            height: 79px;
        }
    }

    @media (min-width: 1107px){

        p {
            font-size: 25px;
        }

        .line {
            
            padding-top: 19px;
        }

    }

    @media (min-width: 1107px) {
        .paragraphIntro {
            padding-top: 5em;
        }

        .values {
            padding-top: 5em;
        }
    }
    
</style>