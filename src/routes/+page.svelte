<script lang="ts">
	import PP from '../assets/PP.png';
	import TpRech from '../assets/grand-plongeon-dans-la-vectorisation-de-mots.pdf';
	import consoEner from '../assets/consommation énergétique du logiciel.pdf';
	import graphisme1 from '../assets/graphisme1.png';
	import graphisme2 from '../assets/graphisme2.png';
	import graphisme3 from '../assets/graphisme3.png';
	import graphisme4 from '../assets/graphisme4.png';
	import graphisme5 from '../assets/graphisme5.png';
	import graphisme6 from '../assets/graphisme6.png';
	import graphisme7 from '../assets/graphisme7.png';
	import graphisme8 from '../assets/graphisme8.png';
	import graphisme9 from '../assets/graphisme9.png';

	function getAge(dateString: string) {
		var today = new Date();
		var birthDate = new Date(dateString);
		var age = today.getFullYear() - birthDate.getFullYear();
		var m = today.getMonth() - birthDate.getMonth();
		if (m < 0 || (m === 0 && today.getDate() < birthDate.getDate())) {
			age--;
		}
		return age;
	}
</script>

<div id="mon-bg" class="min-h-[100vh]">
	<div class="grid gap-3 p-[20px] md:p-[50px] lg:grid-cols-3 xl:p-[200px]">
		<div class="grid-row-subgrid col-span-1 flex flex-col justify-between gap-3">
			<div class="col-span-2 aspect-square overflow-hidden rounded-full border-2 bg-white/20">
				<img src={PP} alt="Valentin Regnault" class="h-full w-full object-contain" />
			</div>
			<div class="">
				<h1 class="col-span-2 row-span-1 text-center font-bold lg:text-5xl">VALENTIN REGNAULT</h1>
				<h3 class="text-center lg:text-3xl">CV Numérique</h3>
			</div>

			<div class="card card-bordered col-span-2 row-span-2 border-2 bg-white/20">
				<div class="card-body">
					<h2 class="card-title text-lg font-bold">Bonjour 👋</h2>
					<p>
						Je suis étudiant en informatique, passionné par la programmation depuis le collège.
						Conscient des dérives du numérique (fake news, surconsommation d'énergie, bulles de
						filtre, produits addictifs, atteintes à la vie privée...), je m'engage et me forme pour
						un numérique responsable : un numérique durable, juste et désirable.
					</p>
				</div>
			</div>

			<!-- age -->
			<div class="card stats card-bordered col-span-2 row-span-1 bg-white/20">
				<div class="stat">
					<div class="stat-title">Age</div>
					<div class="stat-value">{getAge('April 6, 2004')} ans</div>
					<div class="stat-desc">6 avril 2004</div>
				</div>
			</div>
			<div class="grow"></div>
		</div>

		<div class="col-span-1 flex flex-col gap-3">
			<!-- Projets -->
			<div class="border-ht2 card card-bordered col-span-5 row-span-5 bg-white/20">
				<div class="card-body">
					<div class="join join-vertical w-full">
						<blockquote>
							<svg
								class="mb-4 h-8 w-8 text-gray-400 dark:text-gray-600"
								aria-hidden="true"
								xmlns="http://www.w3.org/2000/svg"
								fill="currentColor"
								viewBox="0 0 18 14"
							>
								<path
									d="M6 0H2a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3H2a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Zm10 0h-4a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3h-1a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Z"
								/>
							</svg>
							<p class="text-xl font-semibold italic text-gray-900 dark:text-white">
								"Choisissez un travail que vous aimez et vous n'aurez pas à travailler un seul jour
								de votre vie"
							</p>
							<p class="text-end">- Confucius</p>
						</blockquote>
						<p>
							Nous passons environ 100 000 heures de notre vie à travailler. Confucius nous invite à
							choisir un métier qui nous plaît, mais je pense qu'il est encore plus essentiel de se
							sentir utile. C'est pourquoi je m'efforce de concilier ma passion pour l'informatique
							avec mes valeurs. Je souhaite travailler pour des organisations à impact, engagée, qui
							portent une vision du numérique responsable. Pour moi, le numérique est souvent
							utilisé de manière néfaste, mais est aussi nécessaire dans un monde plus durable. Je
							cherche donc à contribuer à des projets d'informatique qui sont utiles, accessibles,
							qui consomment le minimum d'énergie et de ressources, qui respectent la vie privée des
							utilisateurs et qui contribuent à les rendre plus critiques et plus engagés.
						</p>
					</div>
				</div>
			</div>

			<!-- Projets -->
			<div class="border-ht2 card card-bordered col-span-5 row-span-5 bg-white/20">
				<div class="card-body">
					<h1 class="card-title">Mes projets</h1>
					<div class="join join-vertical w-full">
						<div class="collapse join-item collapse-arrow border border-base-300">
							<input type="radio" name="my-accordion-4" />
							<div class="collapse-title text-xl font-medium">Clone de Slay The Spire</div>
							<div class="collapse-content">
								<p>
									Un clone du jeu Slay the Spire réalisé en Java dans le cadre du cours de
									programmation orientée objet en deuxième année de licence. L'intérêt principal de
									ce projet résidait dans les choix d'architecture pour concevoir ce jeu. Vous
									pouvez retrouver le détail des solutions choisies :
								</p>
								<br />
								<a
									class="btn"
									href="https://github.com/ValentinRegnault/Projet-PO/tree/main/Projet-PO"
								>
									Voir le projet
								</a>
							</div>
						</div>
						<div class="collapse join-item collapse-arrow border border-base-300">
							<input type="radio" name="my-accordion-4" />
							<div class="collapse-title text-xl font-medium">Pidec</div>
							<div class="collapse-content">
								<p>
									Un calculateur de la n-ième décimal de Pi, traduction de l'implémentation en C++
									de Xavier Gourdon.
								</p>
								<br />
								<a href="https://github.com/ValentinRegnault/pidec" class="btn">Voir le projet</a>
							</div>
						</div>
						<div class="collapse join-item collapse-arrow border border-base-300">
							<input type="radio" name="my-accordion-4" />
							<div class="collapse-title text-xl font-medium">Site d'inscription Hack Ta Fac</div>
							<div class="collapse-content">
								<p>
									J'ai été responsable de l'organisation d'HackTaFac, une compétition de
									programmation organisée par La Palme, le BDE de l'ISTIC. En plus de coordonner une
									équipe d'une quinzaine de bénévoles, j'ai également pris en charge la
									communication de l'événement, notamment en réalisant ce site d'inscription dédié.
								</p>
								<br />
								<a class="btn" href="https://github.com/bde-palme/nuitInfo2023">Voir le projet</a>
							</div>
						</div>
						<div class="collapse join-item collapse-arrow border border-base-300">
							<input type="radio" name="my-accordion-4" />
							<div class="collapse-title text-xl font-medium">Hébergeur solaire 🌞</div>
							<div class="collapse-content">
								<p>
									<b>[EN COURS]</b> Je suis responsable du projet d’hébergeur solaire au sein de l’association
									d’électronique de l’ISTIC, Robocoop. Ce projet consiste en un mini-CMS développé en
									Rust, destiné aux sites web des associations de l’université, hébergé sur un Raspberry
									Pi alimenté par un panneau solaire.
								</p>
								<br />
								<a class="btn" href="https://gitlab2.istic.univ-rennes1.fr/robocoop/web-solaire">
									Voir le projet
								</a>
							</div>
						</div>
					</div>
				</div>
			</div>

			<!-- Documents -->
			<div class="card card-body card-bordered col-span-5 bg-white/20">
				<h1 class="card-title">Mes écrits</h1>

				<div class="join join-vertical w-full">
					<div class="collapse join-item collapse-arrow border border-base-300">
						<input type="radio" name="my-accordion-4" checked />
						<div class="collapse-title text-xl font-medium">
							Grand plongeon dans la vectorisation de mots
						</div>
						<div class="collapse-content">
							<p>
								Un rapport sur la vectorisation de mot (plongement lexical), réalisé dans la cadre
								du projet de recherche documentaire en licence 2.
							</p>
							<br />
							<a class="btn" href={TpRech}>Télécharger le rapport </a>
						</div>
					</div>
					<div class="collapse join-item collapse-arrow border border-base-300">
						<input type="radio" name="my-accordion-4" />
						<div class="collapse-title text-xl font-medium">
							Rapport sur la consommation énergétique du logiciel
						</div>
						<div class="collapse-content">
							<p>
								Un rapport sur la consommation énergétique du logiciel, réalisé dans le cadre de la
								mineure numérique éco-responsable.
							</p>
							<br />
							<a href={consoEner} download class="btn">Télécharger le rapport</a>
						</div>
					</div>
				</div>
			</div>
		</div>

		<!-- Timeline -->
		<ul
			class="card card-body timeline card-bordered timeline-vertical timeline-compact timeline-snap-icon col-span-1 flex flex-col gap-3 bg-white/20"
		>
			<li>
				<div class="timeline-middle">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 20 20"
						fill="currentColor"
						class="h-5 w-5"
					>
						<path
							fill-rule="evenodd"
							d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
							clip-rule="evenodd"
						/>
					</svg>
				</div>
				<div class="timeline-end mb-10">
					<time class="font-mono italic">2022</time>
					<div class="text-lg font-black">Baccalauréat</div>
					J'ai obtenu mon bac général mention très bien, section euro, avec les spécialités Mathématiques,
					Sciences de l'ingénieur et Physique-Chimie, et l'option Maths expertes.
				</div>
				<hr />
			</li>
			<li>
				<hr />
				<div class="timeline-middle">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 20 20"
						fill="currentColor"
						class="h-5 w-5"
					>
						<path
							fill-rule="evenodd"
							d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
							clip-rule="evenodd"
						/>
					</svg>
				</div>
				<div class="timeline-end">
					<time class="font-mono italic">2023</time>
					<div class="text-lg font-black">Licence 1</div>
					J'ai débuté mes études à l'ISTIC, Université de Rennes, en licence d'informatique et électronique.
					J'ai terminé l'année avec une moyenne de 18,19, ce qui m'a permis d'être major de ma promotion
					💪.
					<div class="text-lg font-black">Élections étudiantes</div>
					Je suis élu au Conseil de la Formation et de la Vie Étudiante au suffrage direct pour représenter
					les étudiants et étudiantes de mon université. Je m'engage particulièrement dans les commissions
					liées à la vie étudiante et associative, où je défends notamment les demandes de subventions
					des associations.
					<div class="text-lg font-black">Ambassadeurs des Transitions</div>
					À la rentrée 2023, j'obtient le poste d'Ambassadeur des Transitions, pour lequel je suis rémunéré
					par l'Université de Rennes. Ma mission consiste à sensibiliser les étudiants et étudiantes
					aux questions environnementales et sociales. J'organise des conférences, des débats, et soutiens
					des associations.
					<div class="text-lg font-black">Stage à l'étude SEGUR</div>
					<span>J'effectue un stage à </span>
					<a class="underline" href="https://www.segur.eu/">l'étude SEGUR</a>, et je développe un
					outils de génération d'arbres généalogiques, avec des technologies WEB (React, D3.js).
				</div>
				<hr />
			</li>
			<li>
				<hr />
				<div class="timeline-middle">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 20 20"
						fill="currentColor"
						class="h-5 w-5"
					>
						<path
							fill-rule="evenodd"
							d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
							clip-rule="evenodd"
						/>
					</svg>
				</div>
				<div class="timeline-end mb-10">
					<time class="font-mono italic">2024</time>
					<div class="text-lg font-black">Bénévolat</div>
					Je suis devenu membre des conseils d’administration de deux associations de l’ISTIC : La Palme
					(BDE) et Robocoop (électronique/robotique). Déjà très investi dans la vie associative, cela
					marque une nouvelle étape dans mon engagement.
					<div class="text-lg font-black">Licence 2</div>
					Toujours sur ma lancée, j'ai obtenu ma deuxième année de licence avec une moyenne générale
					de 16,35, me plaçant deuxième de ma promotion.
					<div class="text-lg font-black">Étudiant Relais Info</div>
					J'obtient le job d'Étudiant Relais Info, qui consiste à communiquer auprès des étudiants sur
					les actualités universitaire. Je me lance dans une année de publication hebdomadaire puis bimensuelles
					de vidéos pour résumer l'actualité.<a
						class="underline"
						href="https://www.instagram.com/p/DDoZ0-is6cc/"
					>
						Voir un exemple.
					</a>
					<br />
					<div class="text-lg font-black">Stage chez Treebal</div>
					<span>J'effectue un stage chez </span>
					<a class="underline" href="https://www.treebal.green/">Treebal</a>, qui conçoit une
					messagerie alternative dans le genre de whatsapp, écoconçue, sobre et souveraine.
					<div class="text-lg font-black">Break The Code</div>
					Avec mes coéquipiers Nathan et Rémi, nous décrochons la première place lors de la compétition
					d'algorithmie Break The Code, organisée par Sopra Steria à Rennes.
				</div>
				<hr />
			</li>
		</ul>

		<div class="border-ht2 card card-bordered bg-white/20 p-10 sm:col-span-3">
			<h1 class="card-title">Graphisme</h1>
			<p>
				Passionné de graphisme, je réalise de nombreux visuels dans le cadre de mes activités
				associatives. En voici quelques examples :
			</p>
			<div class="flex flex-row flex-wrap gap-5">
				<img src={graphisme1} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme2} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme3} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme4} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme5} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme6} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme7} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme8} alt="" class="w-[400px] border-4 border-[black]" />
				<img src={graphisme9} alt="" class="w-[400px] border-4 border-[black]" />
			</div>
		</div>
	</div>
</div>

<style>
	#mon-bg {
		background: rgb(110, 235, 251);
		background: -moz-linear-gradient(
			54deg,
			rgba(110, 235, 251, 1) 0%,
			rgba(255, 255, 255, 1) 23%,
			rgba(255, 255, 255, 1) 64%,
			rgba(122, 255, 185, 1) 100%
		);
		background: -webkit-linear-gradient(
			54deg,
			rgba(110, 235, 251, 1) 0%,
			rgba(255, 255, 255, 1) 23%,
			rgba(255, 255, 255, 1) 64%,
			rgba(122, 255, 185, 1) 100%
		);
		background: linear-gradient(
			54deg,
			rgba(110, 235, 251, 1) 0%,
			rgba(255, 255, 255, 1) 23%,
			rgba(255, 255, 255, 1) 64%,
			rgba(122, 255, 185, 1) 100%
		);
		filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#6eebfb",endColorstr="#7affb9",GradientType=1);
	}
</style>
