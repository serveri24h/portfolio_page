<script>

    // server box
    let box_width = 300;
    let box_height = 75;
    let box_distance = 90;
    let x_offset = 50;
    let y_offset = 150

    // server buttons
    let button_w = 15;
    let button_h = 10;
    let button_distance = 20;
    let button_offset = 12

</script>


<logo>
    <svg width="400" height="400" viewBox="0 0 400 500">
        <circle cx="200" cy="100" r="10" class="antenna-knob"/>
        <line x1="200" y1="450" x2="200" y2="100" class="backbone"/>
        <line x1="0" y1="500" x2="200" y2="450" class="backbone"/>
        <line x1="400" y1="500" x2="200" y2="450" class="backbone"/>
        <circle cx="200" cy="100" r="0" class="antenna-signal"/>

        {#each [0,1,2] as i}
            <circle cx="{x_offset}" cy="{y_offset+box_distance*i+box_height/2}" r={box_height/2} class="serv-box"/>
            <rect x="{x_offset}" y="{y_offset+box_distance*i}" width="{box_width}" height="{box_height}" class="serv-box"/>
            <circle cx="{x_offset+box_width}" cy="{y_offset+box_distance*i+box_height/2}" r={box_height/2} class="serv-box"/>
            {#each [0,1,2,3] as bx}
                {#each [0,1,2] as by}
                    <rect x="{x_offset+button_offset+bx*button_distance}" y="{y_offset+button_offset+box_distance*i+button_distance*by}" width="{button_w}" height="{button_h}" class="serv-button" id="button-{i}-{3*bx+by}"/>
                {/each}
            {/each}
            <circle cx="{x_offset+box_width-70}" cy="{y_offset+box_distance*i+box_height/2}" r={box_height/4} class="inner-circle"/>
            <circle cx="{x_offset+box_width-20}" cy="{y_offset+box_distance*i+box_height/2}" r={box_height/4} class="inner-circle"/>
        {/each} 
    </svg>  
</logo>

<style>
    
    :root {
        --box-color1: #101010;
        --box-color2: #a40000;
        --box-color3: #2f6900;

        --backbone-color: #d0d0d0;
    }

    @keyframes antenna-anim {
        0% {
            r: 10px;
        }

        50% {
            r: 20px;
        }

        100% {
            r: 10px;
        }
    }

    .antenna-knob {
        fill: var(--backbone-color);
        animation-name: antenna-anim;
        animation-duration: 1s;
        animation-iteration-count: infinite;
    }

    @keyframes signal-anim {
        0% {
            r: 0px;
        }

        100% {
            r: 100px;
            stroke-width: 0px;

        }
    }

    .antenna-signal {
        fill: none;
        stroke: #a40000;
        stroke-width: 4px;
        animation-name: signal-anim;
        animation-duration: 1s;
        animation-iteration-count: infinite;
    }

    .backbone {
        stroke: var(--backbone-color);
        stroke-width: 10px;
    }

    .serv-box {
        fill: #9a9a9a;
    }

    @keyframes animate_boxes {

        0% {
            fill: var(--box-color1);
        }

        50% {
            fill: var(--box-color1);
        }

        75% {
            fill: #6f2abe;
        }

        100% {
            fill: var(--box-color1);
        }
    }

    .serv-button {
        transition: transform 2s;
        fill: box-color1;
        animation-name: animate_boxes;
        animation-duration: 5s;
        animation-iteration-count: infinite;
    }

    .inner-circle {
        fill: none;
        stroke: #101010;
        stroke-width: 0.2em;
    }

</style>