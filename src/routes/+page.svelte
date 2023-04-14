<script>
	import Header from "../Header.svelte";
	import Footer from "../Footer.svelte";
	let pairs = [
		{
			imgSrc: "/images/Danai Gurira _ Dominique Thorne.jpg",
			imgAlt: "",
			imgClass: "lg-br md-br sm-br",
			legend: "Danai Gurira",
			legendOccupation: "Playwright & Actress",
			legendNewLine: false,
			heir: "Dominique Thorne",
			heirOccupation: "Actress",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/danai-gurira-dominique-thorne.html",
		},
		{
			imgSrc: "/images/Graciela Iturbide _ Maya Goded.jpg",
			imgAlt: "",
			imgClass: "lg-b md-b sm-bl",
			legend: "Graciela Iturbide",
			legendOccupation: "Photographer",
			legendNewLine: false,
			heir: "Maya Goded",
			heirOccupation: "Photographer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/graciela-iturbide-maya-goded.html",
		},
		{
			imgSrc: "/images/Paula Vogel _ Sarah Ruhl.jpg",
			imgAlt: "",
			imgClass: "lg-b md-bl sm-br",
			legend: "Paula Vogel",
			legendOccupation: "Playwright & Writer",
			legendNewLine: false,
			heir: "Sarah Ruhl",
			heirOccupation: "Playwright & Writer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/paula-vogel-sarah-ruhl.html",
		},
		{
			imgSrc: "",
			imgAlt: "",
			imgClass: "lg-bl md-br sm-bl",
			legend: "Shirin Neshat",
			legendOccupation: "visual artist & filmmaker",
			legendNewLine: false,
			heir: "Emel Mathlouthi",
			heirOccupation: "singer-songwriter",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/shirin-neshat-emel-mathlouthi.html",
		},
		{
			imgSrc: "/images/Margaret Cho _ Atsuko Okatsuka.jpg",
			imgAlt: "",
			imgClass: "lg-r md-b sm-br",
			legend: "margaret cho",
			legendOccupation: "comedian & actress",
			legendNewLine: false,
			heir: "atsuko okatsuka",
			heirOccupation: "comedian",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/margaret-cho-atsuko-okatsuka.html",
		},
		{
			imgSrc: "/images/Ulla Johnson _ Raven Leilani.jpg",
			imgAlt: "",
			imgClass: "lg-b md-l sm-bl",
			legend: "ulla johnson",
			legendOccupation: "fashion designer",
			legendNewLine: false,
			heir: "raven leilani",
			heirOccupation: "writer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/ulla-johnson-raven-leilani.html",
		},
		{
			imgSrc: "/images/Mira Nair _ Aneeth Arora.jpg",
			imgAlt: "",
			imgClass: "lg-b md-r sm-br",
			legend: "mira nair",
			legendOccupation: "filmmaker",
			legendNewLine: false,
			heir: "aneeth arora",
			heirOccupation: "textile maker & fashion designer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/mira-nair-aneeth-arora.html",
		},
		{
			imgSrc: "/images/Jeanette Winterson _ Eleanor Shearer.jpg",
			imgAlt: "",
			imgClass: "lg-l md-b sm-bl",
			legend: "jeanette winterson",
			legendOccupation: "writer",
			legendNewLine: false,
			heir: "eleanor shearer",
			heirOccupation: "writer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/jeanette-winterson-eleanor-shearer.html",
		},
		{
			imgSrc: "/images/Gina Prince-Bythewood _ Thuso Mbedu.jpg",
			imgAlt: "",
			imgClass: "lg-r md-l sm-br",
			legend: "gina prince-bythewood",
			legendOccupation: "screenwriter & director",
			legendNewLine: false,
			heir: "thuso mbedu",
			heirOccupation: "actress",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/gina-prince-bythewood-thuso-mbedu.html",
		},
		{
			imgSrc: "/images/Juliette Lewis _ Sophie Thatcher.jpg",
			imgAlt: "",
			imgClass: "lg-b md-r sm-bl",
			legend: "juliette lewis",
			legendOccupation: "musician & actress",
			legendNewLine: false,
			heir: "sophie thatcher",
			heirOccupation: "actress",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/juliette-lewis-sophie-thatcher-yellowjackets.html",
		},
		{
			imgSrc: "/images/Joy Harjo _ Layli Long Soldier.jpg",
			imgAlt: "",
			imgClass: "lg-b md-t sm-br",
			legend: "joy harjo",
			legendOccupation: "poet & writer",
			legendNewLine: false,
			heir: "layli long soldier",
			heirOccupation: "poet & writer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/joy-harjo-layli-long-soldier.html",
		},
		{
			imgSrc: "",
			imgAlt: "",
			imgClass: "lg-l md-l sm-bl",
			legend: "denyce graves",
			legendOccupation: "opera singer & director",
			legendNewLine: false,
			heir: "symone harcum",
			heirOccupation: "opera singer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/denyce-graves-symone-harcum.html",
		},
		{
			imgSrc: "/images/Anna Deavere Smith _ Michela Marie Lerman.jpg",
			imgAlt: "",
			imgClass: "lg-r md-r sm-br",
			legend: "anna deavere smith",
			legendOccupation: "PLAYWRIGHT & actress",
			legendNewLine: false,
			heir: "michela marino lerman",
			heirOccupation: "tap dancer, musician, & choreographer",
			heirNewLine: true,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/anna-deavere-smith-michela-marino-lerman.html",
		},
		{
			imgSrc: "/images/Margaret Atwood _ Mona Awad.jpg",
			imgAlt: "",
			imgClass: "lg-r md-l sm-bl",
			legend: "margaret atwood",
			legendOccupation: "writer",
			legendNewLine: false,
			heir: "mona awad",
			heirOccupation: "writer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/margaret-atwood-mona-awad.html",
		},
		{
			imgSrc: "/images/Sharon D Clarke _ Alexia Khadime.jpg",
			imgAlt: "",
			imgClass: "lg-b md-l sm-br",
			legend: "sharon d clarke",
			legendOccupation: "actress",
			legendNewLine: false,
			heir: "alexia khadime",
			heirOccupation: "actress",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/sharon-d-clarke-alexia-khadime.html",
		},
		{
			imgSrc: "/images/Wu Tsang _ Klein.jpg",
			imgAlt: "",
			imgClass: "lg-l md-tr sm-bl",
			legend: "wu tsang",
			legendOccupation: "multidisciplinary artist",
			legendNewLine: false,
			heir: "klein",
			heirOccupation: "musician & filmmaker",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/wu-tsang-klein.html",
		},
		{
			imgSrc: "/images/Gabriela Camara _ Monica Lopez Santiago.jpg",
			imgAlt: "",
			imgClass: "lg-r md-t sm-br",
			legend: "gabriela cámara",
			legendOccupation: "chef",
			legendNewLine: false,
			heir: "monica lópez santiago",
			heirOccupation: "chef",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/gabriela-camara-monica-lopez-santiago.html",
		},
		{
			imgSrc: "/images/Marina Abramovic _ Sondra Radvanovsky.jpg",
			imgAlt: "",
			imgClass: "lg-tr md-tl sm-bl",
			legend: "marina abramović",
			legendOccupation: "conceptual artist",
			legendNewLine: false,
			heir: "sondra radvanovsky",
			heirOccupation: "opera singer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/marina-abramovic-sondra-radvanovsky.html",
		},
		{
			imgSrc: "/images/Tourmaline _ Xoai Pham.jpg",
			imgAlt: "",
			imgClass: "lg-l md-tr sm-br",
			legend: "tourmaline",
			legendOccupation: "visual artist",
			legendNewLine: false,
			heir: "xoái phạm",
			heirOccupation: "multidisciplinary artist",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/tourmaline-xoai-pham.html",
		},
		{
			imgSrc: "/images/Sigrid Nunez _ Weike Wang.jpg",
			imgAlt: "",
			imgClass: "lg-l md-tl sm-bl",
			legend: "sigrid nunez",
			legendOccupation: "writer",
			legendNewLine: false,
			heir: "weike wang",
			heirOccupation: "writer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/sigrid-nunez-weike-wang.html",
		},
		{
			imgSrc: "/images/Ruthie Rogers _ Nina Raine.jpg",
			imgAlt: "",
			imgClass: "lg-r md-l sm-tr",
			legend: "ruth rogers",
			legendOccupation: "chef",
			legendNewLine: false,
			heir: "nina raine",
			heirOccupation: "playwright & director",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/ruth-rogers-nina-raine.html",
		},
		{
			imgSrc: "/images/Wangechi Mutu _ Priscella Aleman.jpg",
			imgAlt: "",
			imgClass: "lg-tr md-tr sm-tl",
			legend: "wangechu mutu",
			legendOccupation: "multimedia artist",
			legendNewLine: false,
			heir: "priscilla aleman",
			heirOccupation: "multimedia artist",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/wangechi-mutu-priscilla-aleman.html",
		},
		{
			imgSrc: "/images/Bernardine Evaristo _ Lynette Linton.jpg",
			imgAlt: "",
			imgClass: "lg-tl md-tl sm-tr",
			legend: "bernardine evaristo",
			legendOccupation: "writer",
			legendNewLine: false,
			heir: "lynette linton",
			heirOccupation: "playwright & director",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/bernardine-evaristo-lynette-linton.html",
		},
		{
			imgSrc: "/images/Joan Baez _ Lana Del Rey.jpg",
			imgAlt: "",
			imgClass: "lg-l md-tl sm-tl",
			legend: "joan baez",
			legendOccupation: "singer-songwriter & visual artist",
			legendNewLine: false,
			heir: "lana del rey",
			heirOccupation: "singer-songwriter",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/lana-del-rey-joan-baez.html",
		},
		{
			imgSrc: "",
			imgAlt: "",
			imgClass: "lg-tr md-tr sm-tr",
			legend: "marlee matlin",
			legendOccupation: "actress",
			legendNewLine: false,
			heir: "teyana taylor",
			heirOccupation: "singer-songwriter & actress",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/marlee-matlin-teyana-taylor.html",
		},
		{
			imgSrc: "/images/Maria Grazia Chiuri _ Zadie Xa.jpg",
			imgAlt: "",
			imgClass: "lg-t md-t sm-tl",
			legend: "maria grazia chiuri",
			legendOccupation: "fashion designer",
			legendNewLine: false,
			heir: "zadie xa",
			heirOccupation: "interdisciplinary artist",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/maria-grazia-chiuri-zadie-xa.html",
		},
		{
			imgSrc: "/images/Emily Watson _ Aisling Franciosi.jpg",
			imgAlt: "",
			imgClass: "lg-t md-tl sm-tr",
			legend: "emily watson",
			legendOccupation: "actress",
			legendNewLine: false,
			heir: "aisling franciosi",
			heirOccupation: "actress",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/emily-watson-aisling-franciosi.html",
		},
		{
			imgSrc: "/images/Howardena Pindell _ Melissa Cody.jpg",
			imgAlt: "",
			imgClass: "lg-tl md-tr sm-tl",
			legend: "howardena pindell",
			legendOccupation: "painter",
			legendNewLine: false,
			heir: "melissa cody",
			heirOccupation: "textile artist",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/howardena-pindell-melissa-cody.html",
		},
		{
			imgSrc: "/images/Naomi Watts _ Elle Fanning.jpg",
			imgAlt: "",
			imgClass: "lg-tr md-t sm-tr",
			legend: "naomi watts",
			legendOccupation: "actress",
			legendNewLine: false,
			heir: "elle fanning",
			heirOccupation: "actress",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/naomi-watts-elle-fanning.html",
		},
		{
			imgSrc: "/images/Rita Dove _ Safiya Sinclair.jpg",
			imgAlt: "",
			imgClass: "lg-t md-tl sm-tl",
			legend: "rita dove",
			legendOccupation: "poet & writer",
			legendNewLine: false,
			heir: "safiya sinclair",
			heirOccupation: "poet & writer",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/rita-dove-safiya-sinclair.html",
		},
		{
			imgSrc: "",
			imgAlt: "",
			imgClass: "lg-t md-tr sm-tr",
			legend: "cheryl james and sandra denton, a.k.a. Salt-N-Pepa",
			legendOccupation: "musicians",
			legendNewLine: true,
			heir: "issa rae",
			heirOccupation: "actress, producer, and screenwriter",
			heirNewLine: false,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/salt-n-pepa-issa-rae.html",
		},
		{
			imgSrc: "/images/Madhur Jaffrey _ Japanese Breakfast.jpg",
			imgAlt: "",
			imgClass: "lg-tl md-t sm-tl",
			legend: "madhur jaffrey",
			legendOccupation: "actress & writer",
			legendNewLine: false,
			heir: "michell zauner, a.k.a. japenese breakfast",
			heirOccupation: "singer-songwriter and writer",
			heirNewLine: true,
			articleLink:
				"https://www.nytimes.com/2023/04/20/t-magazine/japanese-breakfast-madhur-jaffrey.html",
		},
	];
</script>

<section class="wrapper">
	<Header />
	<div class="lh-grid">
		{#each pairs as pair, i}
			<a href={pair.articleLink}>
				<div class="lh-grid-item">
					<div class="grid-item-wrapper">
						<div class="grid-underline-row">
							<span class="legend-text">{`${pair.legend}, `}</span>
							{#if !pair.legendNewLine}
								<span class="small-text">{`${pair.legendOccupation}`}</span>
							{/if}
						</div>
						{#if pair.legendNewLine}
							<div class="grid-underline-row">
								<span class="small-text">{`${pair.legendOccupation}`}</span>
							</div>
						{/if}
						<div class="grid-underline-row">
							<span class="small-text">and</span>
							<span class="heir-text">{`${pair.heir}, `}</span>
							{#if !pair.heirNewLine}
								<span class="small-text">{`${pair.heirOccupation}`}</span>
							{/if}
						</div>
						{#if pair.heirNewLine}
							<div class="grid-underline-row">
								<span class="small-text">{`${pair.heirOccupation}`}</span>
							</div>
						{/if}
					</div>
					<img class={pair.imgClass} src={pair.imgSrc} />
				</div>
			</a>
		{/each}
	</div>
	<Footer />
</section>

<style>
	/* GRID COLUMNS ONLY: */
	@media only screen and (max-width: 730px) {
		.lh-grid {
			display: grid;
			grid-template-columns: 1fr;
		}
	}
	@media only screen and (min-width: 731px) and (max-width: 1200px) {
		.lh-grid {
			display: grid;
			grid-template-columns: 1fr 1fr;
		}
		.grid-item-wrapper + img.sm-t {
			bottom: 100px;
		}
		.grid-item-wrapper + img.sm-tr {
			bottom: 100px;
			left: 70%;
		}
		.grid-item-wrapper + img.sm-tl {
			bottom: 100px;
			right: 70%;
		}
		.grid-item-wrapper + img.sm-b {
			top: 100px;
		}
		.grid-item-wrapper + img.sm-br {
			top: 100px;
			left: 70%;
		}
		.grid-item-wrapper + img.sm-bl {
			top: 70px;
			right: 70%;
		}
		.grid-item-wrapper + img.sm-l {
			right: 100%;
		}
		.grid-item-wrapper + img.sm-r {
			left: 100%;
		}
	}
	@media only screen and (min-width: 1201px) and (max-width: 1449px) {
		.lh-grid {
			display: grid;
			grid-template-columns: 1fr 1fr 1fr;
		}
		.grid-item-wrapper + img.md-t {
			bottom: 100px;
		}
		.grid-item-wrapper + img.md-tr {
			bottom: 100px;
			left: 70%;
		}
		.grid-item-wrapper + img.md-tl {
			bottom: 100px;
			right: 70%;
		}
		.grid-item-wrapper + img.md-b {
			top: 100px;
		}
		.grid-item-wrapper + img.md-br {
			top: 100px;
			left: 70%;
		}
		.grid-item-wrapper + img.md-bl {
			top: 70px;
			right: 70%;
		}
		.grid-item-wrapper + img.md-l {
			right: 100%;
		}
		.grid-item-wrapper + img.md-r {
			left: 100%;
		}
	}
	@media only screen and (min-width: 1450px) {
		.lh-grid {
			display: grid;
			grid-template-columns: 1fr 1fr 1fr 1fr;
		}
		.grid-item-wrapper + img.lg-t {
			bottom: 100px;
		}
		.grid-item-wrapper + img.lg-tr {
			bottom: 100px;
			left: 70%;
		}
		.grid-item-wrapper + img.lg-tl {
			bottom: 100px;
			right: 70%;
		}
		.grid-item-wrapper + img.lg-b {
			top: 100px;
		}
		.grid-item-wrapper + img.lg-br {
			top: 100px;
			left: 70%;
		}
		.grid-item-wrapper + img.lg-bl {
			top: 70px;
			right: 70%;
		}
		.grid-item-wrapper + img.lg-l {
			right: 100%;
		}
		.grid-item-wrapper + img.lg-r {
			left: 100%;
		}
	}

	/* SMALL */
	@media only screen and (max-width: 740px) {
		.legend-text,
		.heir-text {
			font-size: 16px;
		}
		.legend-text {
			font-family: "KipCondensedBold";
		}
		.heir-text {
			font-family: "FactCondensedBold";
		}
		.grid-item-wrapper + img {
			display: none;
		}
		.lh-grid-item {
			height: auto;
			padding-top: 15px;
			padding-bottom: 15px;
			line-height: 1.1;
		}
		.grid-underline-row::after {
			display: none;
		}
		.lh-grid-item {
			position: relative;
			border-top: 1px black dashed;
			display: flex;
			align-items: center;
			justify-content: center;
		}
	}
	/* MEDIUM */
	@media only screen and (min-width: 741px) and (max-width: 850px) {
		.legend-text,
		.heir-text {
			font-size: 17px;
		}
		.legend-text {
			font-family: "KipCondensedRegular";
		}
		.heir-text {
			font-family: "FactCondensedRegular";
		}
		.grid-item-wrapper + img {
			opacity: 0%;
			width: 400px;
			height: auto;
			position: absolute;
			z-index: 50;
			/* top: 70px;
			left: 0px; */
			transition: opacity 0.2s linear;
			pointer-events: none;
		}
		.grid-item-wrapper:hover + img {
			opacity: 100%;
		}
		.lh-grid-item {
			height: 80px;
			line-height: 1.3;
		}
		.grid-underline-row::after {
			content: "";
			position: absolute;
			bottom: 0;
			left: 0;
			width: 100%;
			height: 3px;
			background-color: #a19be8;
			opacity: 0;
			transition: opacity 300ms, transform 300ms;
			transform: translate3d(-100%, 0, 0);
		}
		.grid-item-wrapper:hover > .grid-underline-row::after,
		.grid-item-wrapper:focus > .grid-underline-row::after {
			transform: translate3d(0, 0, 0);
			opacity: 1;
		}
		.lh-grid-item {
			position: relative;
			border-top: 1px black dashed;
			border-bottom: 1px black dashed;
			margin-bottom: -1px;
			display: flex;
			align-items: center;
			justify-content: center;
		}
	}
	/* LARGE */
	@media only screen and (min-width: 851px) {
		.legend-text,
		.heir-text {
			font-size: 17px;
		}
		.legend-text {
			font-family: "KipCondensedRegular";
		}
		.heir-text {
			font-family: "FactCondensedRegular";
		}
		.grid-item-wrapper + img {
			opacity: 0%;
			width: 400px;
			height: auto;
			position: absolute;
			z-index: 50;
			transition: opacity 0.2s linear;
			pointer-events: none;
		}

		.grid-item-wrapper:hover + img {
			opacity: 100%;
		}
		.lh-grid-item {
			height: 80px;
			line-height: 1.3;
		}
		.grid-underline-row::after {
			content: "";
			position: absolute;
			bottom: 0;
			left: 0;
			width: 100%;
			height: 3px;
			background-color: #a19be8;
			opacity: 0;
			transition: opacity 300ms, transform 300ms;
			transform: translate3d(-100%, 0, 0);
		}

		.grid-item-wrapper:hover > .grid-underline-row::after,
		.grid-item-wrapper:focus > .grid-underline-row::after {
			transform: translate3d(0, 0, 0);
			opacity: 1;
		}
		.grid-item-wrapper:hover > .grid-underline-row > .legend-text {
			font-family: "KipCondensedBold";
		}
		.grid-item-wrapper:hover > .grid-underline-row > .heir-text {
			font-family: "FactCondensedBold";
		}
		.lh-grid-item {
			position: relative;
			border-top: 1px black dashed;
			border-bottom: 1px black dashed;
			margin-bottom: -1px;
			display: flex;
			align-items: center;
			justify-content: center;
		}
	}
	/* ALL SCREEN SIZES / GLOBAL */
	:global(*) {
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		box-sizing: border-box;
	}
	:global(body) {
		padding: 0px !important;
		margin: 0px !important;
	}
	a {
		text-decoration: none;
		color: inherit;
	}
	.wrapper {
		background-color: #eeeeee;
	}
	.grid-underline-row {
		text-decoration: none;
		overflow: hidden;
		position: relative;
		width: fit-content;
		text-align: center;
	}
	.grid-item-wrapper {
		text-align: center;
		position: relative;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.legend-text,
	.heir-text,
	.small-text {
		text-transform: uppercase;
	}
	.small-text {
		font-size: 13px;
		font-family: "KipCondensedRegular";
	}

	@font-face {
		font-family: "FactCondensedRegular";
		src: url("/Fact Deck-57 Condensed Regular.otf") format("opentype");
	}
	@font-face {
		font-family: "FactMedium";
		src: url("/Fact Deck-65 Medium.otf") format("opentype");
	}
	@font-face {
		font-family: "FactCondensedMedium";
		src: url("/Fact Deck-67 Condensed Medium.otf") format("opentype");
	}
	@font-face {
		font-family: "FactBold";
		src: url("/Fact Deck-75 Bold.otf") format("opentype");
	}
	@font-face {
		font-family: "FactCondensedBold";
		src: url("/Fact Deck-77 Condensed Bold.otf") format("opentype");
	}
	@font-face {
		font-family: "KipRegular";
		src: url("/Kippenberger-55 Regular.otf") format("opentype");
	}
	@font-face {
		font-family: "KipCondensedRegular";
		src: url("/Kippenberger-57 Condensed Regular.otf") format("opentype");
	}
	@font-face {
		font-family: "KipBold";
		src: url("/Kippenberger-75 Bold.otf") format("opentype");
	}
	@font-face {
		font-family: "KipCondensedBold";
		src: url("/Kippenberger-77 Condensed Bold.otf") format("opentype");
	}
</style>
