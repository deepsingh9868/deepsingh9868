<!-- original by felix rilling: https://codepen.io/FelixRilling/pen/vNJoMy, edited by reeveng https://github.com/reeveng -->
<svg fill="none" viewBox="0 0 1000 400" width="1000" height="400" xmlns="http://www.w3.org/2000/svg">
	<foreignObject width="100%" height="100%">
		<div xmlns="http://www.w3.org/1999/xhtml">
			<style>
                .container {
                font-family: system-ui, -apple-system, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji';
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                margin: 0;
                width: 100%;
                height: 400px;
                /* background: linear-gradient(-45deg, #fc5c7d, #6a82fb, #05dfd7); */
                background: #333;
                background-size: 600% 400%;
                border-radius: 10px;
                /* color: white; */
                text-align: center;
                }


                h1 {
                text-align: center;
                color: #fff;
                font-size: 5em;
                letter-spacing: 8px;
                font-family: "Lucida Console", Monaco, monospace;	
                font-weight: 400;
                /*Create overlap*/
                
                margin: 0;
                line-height: 0;
                /*Animation*/
                
                animation: glitch1 2.5s infinite;
                }

                h1:nth-child(2) {
                color: #67f3da;
                animation: glitch2 2.5s infinite;
                }

                h1:nth-child(3) {
                color: #f16f6f;
                animation: glitch3 2.5s infinite;
                }
                /*Keyframes*/

                @keyframes glitch1 {
                0% {
                    transform: none;
                    opacity: 1;
                }
                7% {
                    transform: skew(-0.5deg, -0.9deg);
                    opacity: 0.75;
                }
                10% {
                    transform: none;
                    opacity: 1;
                }
                27% {
                    transform: none;
                    opacity: 1;
                }
                30% {
                    transform: skew(0.8deg, -0.1deg);
                    opacity: 0.75;
                }
                35% {
                    transform: none;
                    opacity: 1;
                }
                52% {
                    transform: none;
                    opacity: 1;
                }
                55% {
                    transform: skew(-1deg, 0.2deg);
                    opacity: 0.75;
                }
                50% {
                    transform: none;
                    opacity: 1;
                }
                72% {
                    transform: none;
                    opacity: 1;
                }
                75% {
                    transform: skew(0.4deg, 1deg);
                    opacity: 0.75;
                }
                80% {
                    transform: none;
                    opacity: 1;
                }
                100% {
                    transform: none;
                    opacity: 1;
                }
                }

                @keyframes glitch2 {
                0% {
                    transform: none;
                    opacity: 0.25;
                }
                7% {
                    transform: translate(-2px, -3px);
                    opacity: 0.5;
                }
                10% {
                    transform: none;
                    opacity: 0.25;
                }
                27% {
                    transform: none;
                    opacity: 0.25;
                }
                30% {
                    transform: translate(-5px, -2px);
                    opacity: 0.5;
                }
                35% {
                    transform: none;
                    opacity: 0.25;
                }
                52% {
                    transform: none;
                    opacity: 0.25;
                }
                55% {
                    transform: translate(-5px, -1px);
                    opacity: 0.5;
                }
                50% {
                    transform: none;
                    opacity: 0.25;
                }
                72% {
                    transform: none;
                    opacity: 0.25;
                }
                75% {
                    transform: translate(-2px, -6px);
                    opacity: 0.5;
                }
                80% {
                    transform: none;
                    opacity: 0.25;
                }
                100% {
                    transform: none;
                    opacity: 0.25;
                }
                }

                @keyframes glitch3 {
                0% {
                    transform: none;
                    opacity: 0.25;
                }
                7% {
                    transform: translate(2px, 3px);
                    opacity: 0.5;
                }
                10% {
                    transform: none;
                    opacity: 0.25;
                }
                27% {
                    transform: none;
                    opacity: 0.25;
                }
                30% {
                    transform: translate(5px, 2px);
                    opacity: 0.5;
                }
                35% {
                    transform: none;
                    opacity: 0.25;
                }
                52% {
                    transform: none;
                    opacity: 0.25;
                }
                55% {
                    transform: translate(5px, 1px);
                    opacity: 0.5;
                }
                50% {
                    transform: none;
                    opacity: 0.25;
                }
                72% {
                    transform: none;
                    opacity: 0.25;
                }
                75% {
                    transform: translate(2px, 6px);
                    opacity: 0.5;
                }
                80% {
                    transform: none;
                    opacity: 0.25;
                }
                100% {
                    transform: none;
                    opacity: 0.25;
                }
                }
			</style>
			<div class="container">
                <h1>Hey, I'm Deepak!</h1>
                <h1>Hey, I'm Deepak!</h1>
                <h1>Hey, I'm Deepak!</h1>
            </div>
        </div>
	</foreignObject>
</svg>

<h2 align="center">About me</h2>

```golang
package main

import (
	"fmt"
)

type Bio map[string]string

func main() {
	for k, v := range GetBio() {
		fmt.Printf("%+v: %+v\n", k, v)
	}
}

func GetBio() Bio {
	return Bio{
		"- ⚡ Quick bio:":                    "A kind of metalHead-melomaniac-gearAddict-amateurMusician-traveler-foodLover-gamer-coder-programmer-catLover-sportsAficionado hybrid",
		"- 🔭 I’m currently working on":      "Tredicom as a Senior Software Developer --- UAdeC as a Part Time Teacher",
		"- 🌱 I’m currently learning":        "Golang, MongoDB, RabbitMQ, K8s, GCP (Tech stack from my company) --- Sharpening my Front End Skills for the MERN stack (Personal goal)",
		"- 👯 I’m looking to collaborate on": "Python, Golang and Docker related projects",
		"- 🤔 I’m looking for help with":     "Anything related to what I am currently learning 😅",
		"- 💬 Ask me about":                  "Python, PHP, Laravel, SQL, Software Design & Architecture, Web-Dev and SEO",
		"- 📫 How to reach me:":              "https://github.com/AnhellO#you-can-reach-me-at-alien",
	}
}
```

<h2 align="center">You can reach me at :alien:</h2>

<p align="center">
  <a href="https://dev.to/anhello">
    <img src="https://d2fltix0v2e0sb.cloudfront.net/dev-badge.svg" alt="Angel Santiago Jaime Zavala's DEV Profile" height="30" width="30">
  </a>

  <a href="https://www.linkedin.com/in/angel-santiago-jaime-zavala-601813199/">
    <img src="https://www.vectorlogo.zone/logos/linkedin/linkedin-icon.svg" alt="Angel Santiago Jaime Zavala's LinkedIn Profile" height="30" width="30">
  </a>

  <a href="https://stackoverflow.com/users/2946413/angel-santiago-jaime-zavala?tab=profile">
    <img src="https://www.vectorlogo.zone/logos/stackoverflow/stackoverflow-icon.svg" alt="Angel Santiago Jaime Zavala's Stack Overflow Profile" height="30" width="30">
  </a>

  <a href="https://stackexchange.com/users/3525056/angel-santiago-jaime-zavala">
    <img src="https://www.vectorlogo.zone/logos/stackexchange/stackexchange-icon.svg" alt="Angel Santiago Jaime Zavala's Stack Exchange Profile" height="30" width="30">
  </a>

  <a href="https://stackshare.io/anhello">
    <img src="https://cdn.worldvectorlogo.com/logos/stackshare.svg" alt="Angel Santiago Jaime Zavala's StackShare Profile" height="30" width="30">
  </a>
  
  <a href="https://gitlab.com/AnhellO">
    <img src="https://www.vectorlogo.zone/logos/gitlab/gitlab-icon.svg" alt="Angel Santiago Jaime Zavala's GitLab Profile" height="30" width="30">
  </a>
  
  <a href="https://medium.com/@ajzavala">
    <img src="https://www.vectorlogo.zone/logos/medium/medium-tile.svg" alt="Angel Santiago Jaime Zavala's Medium Profile" height="30" width="30">
  </a>
  
  <a href="https://www.youtube.com/channel/UCPUwB4x7_6Dbvwsnfbe1yiQ">
    <img src="https://www.vectorlogo.zone/logos/youtube/youtube-icon.svg" alt="Angel Santiago Jaime Zavala's YouTube Channel" height="30" width="30">
  </a>
</p>

<h2 align="center">My stack :man_technologist:</h2>

<p align="center">Tools that I use on a daily basis, or that I've used or worked (either much or a bit) with on the past</p>
<p align="center">
  <a href="https://stackshare.io/anhello/my-personal-stack">
    <img src="http://img.shields.io/badge/tech-stack-0690fa.svg?style=flat" alt="AnhellO :: StackShare" />
  </a>
</p>

<h2 align="center">Github stats :bar_chart:</h2>

<h4 align="center">Visitor's count :eyes:</h4>

<p align="center"><img src="https://profile-counter.glitch.me/{AnhellO}/count.svg" alt="AnhellO :: Visitor's Count" /></p>

<h4 align="center">Top langs :tongue:</h4>

<p align="center"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AnhellO&langs_count=10&theme=tokyonight&layout=compact" alt="AnhellO :: Top Langs" /></p>

<h4 align="center">Profile stats :musical_keyboard:</h4>

<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=AnhellO&show_icons=true&theme=synthwave" alt="AnhellO :: Profile Stats" /></p>

<p align="center"><img src="https://thumbs.gfycat.com/GoodnaturedFondGaur-size_restricted.gif" alt="Synthwave" height="300" width="500"></p>


---

⭐️ From [@AnhellO](https://github.com/AnhellO)
