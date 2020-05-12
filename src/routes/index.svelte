<script>
	import Container from 'sveltestrap/src/Container.svelte';
	import Col from 'sveltestrap/src/Col.svelte';
	import Row from 'sveltestrap/src/Row.svelte';
	import Button from 'sveltestrap/src/Button.svelte';
</script>

<svelte:head>
    <title>
        Portfolio | Filip Holčík
    </title>
</svelte:head>

<section class="portfolio-block block-intro">
    <Container>
        <div class="avatar" style="background-image:url(&quot;assets/img/avatars/avatar.jpg&quot;);"></div>
        <div class="about-me">
            <p>
                HI! I'm Filip Holčík, I study at SPŠE Karola Adlera (electrical enegineering).
                I specify mainly on development full-stack apps, PWAs and electron apps. I also learn Flutter, but I am beginner.
            </p>
            <Button outline color="primary" href="contact">
                Contact me
            </Button>
            <Button outline color="success" href="Filip-Holcik-CV.pdf">
                Download my CV
            </Button>
        </div>
    </Container>
</section>
<section class="portfolio-block skills">
    <Container>
        <div class="heading">
            <h2>MY Skills</h2>
        </div>
        <Row>
            <Col md="4">
                <div class="card special-skill-item border-0">
                    <div class="card-header bg-transparent border-0"><i class="icon ion-social-javascript"></i></div>
                    <div class="card-body">
                        <h3 class="card-title">JavaScript</h3>
                        <p class="card-text">I do JavaScript around 2 years. I am capable of coding imperative/declarative code, object-oriented code and I know ES6 as well.</p>
                    </div>
                </div>
            </Col>
            <Col md="4">
                <div class="card special-skill-item border-0">
                    <div class="card-header bg-transparent border-0"><i class="icon ion-social-nodejs"></i></div>
                    <div class="card-body">
                        <h3 class="card-title">Node.js</h3>
                        <p class="card-text">As I sayed before, I am full-stack developer so I have to know back-end too. For back-end I am used to use Node.js (runtime) instead of PHP.</p>
                    </div>
                </div>
            </Col>
            <Col md="4">
                <div class="card special-skill-item border-0">
                    <div class="card-header bg-transparent border-0"><i class="icon ion-social-html5"></i></div>
                    <div class="card-body">
                        <h3 class="card-title">Front-end</h3>
                        <p class="card-text">For front-end I use frameworks, my favorite are Svelte (compiler, competitor to React/Vue) and Sapper (SSG/SSR framework, competitor to Next/Nuxt/Angular).</p>
                    </div>
                </div>
            </Col>
        </Row>
    </Container>
</section>
<section class="portfolio-block skills">
    <Container>
        <div class="heading">
            <h2>Technologies I do</h2>
        </div>
        <Row>
            <Col>
                <div class="card">
                    <div class="card-body">
                        <h4 class="card-title">Front-end</h4>
                        <ul class="list-group">
                            <li class="list-group-item"><span>Principle of frameworks</span></li>
                            <li class="list-group-item"><span>Svelte</span></li>
                            <li class="list-group-item"><span>Boostrap</span></li>
                            <li class="list-group-item"><span>Sass</span></li>
                            <li class="list-group-item"><span>jQuery</span></li>
                        </ul>
                    </div>
                </div>
            </Col>
            <Col>
                <div class="card">
                    <div class="card-body">
                        <h4 class="card-title">Back-end</h4>
                        <ul class="list-group">
                            <li class="list-group-item"><span>Express</span></li>
                            <li class="list-group-item"><span>Firebase</span></li>
                            <li class="list-group-item"><span>Monolithic architecture</span></li>
                            <li class="list-group-item"><span>Nginx</span></li>
                            <li class="list-group-item"><span>Kubernetes (beginner)</span></li>
                        </ul>
                    </div>
                </div>
            </Col>
            <Col>
                <div class="card">
                    <div class="card-body">
                        <h4 class="card-title">Other</h4>
                        <ul class="list-group">
                            <li class="list-group-item"><span>Linux (daily base)</span></li>
                            <li class="list-group-item"><span>Electron</span></li>
                            <li class="list-group-item"><span>Rollup/Webpack</span></li>
                            <li class="list-group-item"><span>Git</span></li>
                            <li class="list-group-item"><span>Flutter (beginner)</span></li>
                        </ul>
                    </div>
                </div>
            </Col>
        </Row>
    </Container>
</section>
<section class="bg-light portfolio-block skills">
    <Container>
        <div class="heading">
            <h2>Tools I work in</h2>
        </div>
        <Row>
            <Col>
                <div class="card">
                    <div class="card-body">
                        <h4 class="card-title">IDEs/Text editors</h4>
                        <ul class="list-group">
                            <li class="list-group-item"><span>WebStorm</span></li>
                            <li class="list-group-item"><span>Atom</span></li>
                            <li class="list-group-item"><span>VIM</span></li>
                            <li class="list-group-item"><span>Android Studio</span></li>
                            <li class="list-group-item"><span>Bootstrap Studio (I use it for sketching)</span></li>
                        </ul>
                    </div>
                </div>
            </Col>
        </Row>
    </Container>
</section>
