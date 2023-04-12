<section class="wrapper">
	<div class="home-link">
		<img src="/handwriting.svg" />
	</div>
	<div class="section-links-wrapper">
		<div class="section-link s1">
			<div class="title">The Artist's Mind</div>
			<div class="subtitle">
				Four writers on what<br />drives, and complicates, creation.
			</div>
		</div>
		<div class="section-link s2">
			<div class="title">Mothers & Daughters</div>
			<div class="subtitle">
				The distinct bonds of an artistic family —<br />biological or otherwise.
			</div>
		</div>
		<div class="section-link s3">
			<div class="title">In Tribute</div>
			<div class="subtitle">
				Five visual artists make portraits for T of<br />the late, great women
				who've inspired them.
			</div>
		</div>
		<div class="section-link s4">
			<div class="title">Legends & Heirs</div>
			<div class="subtitle">
				Artistic icons nominate a younger woman<br />whose work resonates deeply
				with them.
			</div>
		</div>
	</div>
</section>

<style>
	@media only screen and (max-width: 500px) {
		.section-links-wrapper {
			display: grid;
			grid-template-columns: 1fr;
			grid-template-rows: 1fr 1fr 1fr 1fr;
		}
		.home-link,
		.section-links-wrapper {
			width: 100vw;
		}
		.home-link {
			height: 70px;
		}
		.section-link {
			width: 100%;
			height: 100px;
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			text-align: center;
		}
	}
	@media only screen and (min-width: 501px) {
		.section-links-wrapper {
			display: grid;
			grid-template-rows: 1fr;
			grid-template-columns: 1fr 1fr 1fr 1fr;
		}
		.home-link,
		.section-links-wrapper {
			height: 90px;
			width: 100vw;
		}
		.section-link {
			width: 100%;
			height: 100%;
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			text-align: center;
		}
	}
	.wrapper {
		width: 100vw;
	}

	.home-link {
		font-family: "FactMedium";
		background: linear-gradient(180deg, #b9b9b9 0%, #e2e2e0 100%, #e2e2e0 100%);
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.home-link img {
		height: 60%;
		width: auto;
		margin-top: -5px;
	}

	.section-link .subtitle {
		font-family: "FactCondensedMedium";
		line-height: 1.05;
		font-size: 14px;
	}
	.section-link .title {
		font-family: "KipBold";
		font-size: 20px;
		text-transform: uppercase;
		padding-bottom: 3px;
	}
	.s1 {
		background: linear-gradient(360deg, #ffb23e, 0%, #ffd364 100%);
	}
	.s2 {
		background: linear-gradient(360deg, #77ccb6 0%, #9ad88f 100%), #e8f96c;
	}
	.s3 {
		background: linear-gradient(360deg, #efc0b5 0%, #ffaaba 100%);
	}
	.s4 {
		background: linear-gradient(360deg, #a19be8, 0%, #53b2e8 100%);
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
		font-family: "FactCondensedBold";
		src: url("/Fact Deck-77 Condensed Bold.otf") format("opentype");
	}
	@font-face {
		font-family: "FactBold";
		src: url("/Fact Deck-75 Bold.otf") format("opentype");
	}
	@font-face {
		font-family: "KipBold";
		src: url("/Kippenberger-75 Bold.otf") format("opentype");
	}
</style>
