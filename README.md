<p align="center">
<svg width="500" height="80" viewBox="0 0 500 80" xmlns="http://www.w3.org/2000/svg">
    <style>
        .text { font: bold 22px 'Fira Code', monospace; }
        @media (prefers-color-scheme: dark) {
            .text { fill: #FFF; }
        }
        @media (prefers-color-scheme: light) {
            .text { fill: #000; }
        }
    </style>

    <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle" class="text" opacity="0">
        Hello, I'm Srinivas
        <animate attributeName="opacity" values="0;1;1;0" keyTimes="0;0.2;0.8;1" dur="5s" begin="0s" repeatCount="indefinite" />
    </text>
    
    <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle" class="text" opacity="0">
        A Passionate Developer
        <animate attributeName="opacity" values="0;0;1;1;1" keyTimes="0;0.5;0.7;0.9;1" dur="5s" begin="0s" repeatCount="indefinite" />
        <animateMotion path="M 0 0 L -100 -20" dur="0.5s" begin="4.5s" fill="freeze" repeatCount="1">
            <mpath xlink:href="#path1"/>
        </animateMotion>
        <animate attributeName="opacity" values="1;1" dur="0.5s" begin="5s" fill="freeze" repeatCount="1"/>
    </text>
</svg>
</p>
