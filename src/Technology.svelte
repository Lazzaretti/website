<script>
  let technologies = [
    {
      icon: 'img/technology/angular.svg',
      iconAlt: 'angular',
      title: 'Angular',
      text: 'Unser treuer Begleiter seit 10 Jahren. Hilft uns unsere Software für alle Geräte einheitlich anzubieten.',
    },
    {
      icon: 'img/technology/netcore.svg',
      iconAlt: 'dotnet core',
      title: 'dotnet core',
      text: 'Damit es auch hinter der Bühne rund läuft, arbeiten unsere Server mit dotnet 24/7 für unsere Kunden.',
    },
    {
      icon: 'img/technology/nodejs.svg',
      iconAlt: 'node.js',
      title: 'node.js',
      text: 'Kundenideen blitzschnell umsetzen und flexibel bleiben, auch für die kleinen Features im Leben.',
    },
    {
      icon: 'img/technology/postgresql.svg',
      iconAlt: 'postgresql',
      title: 'PostgreSQL',
      text: 'Daten hält PostgreSQL für uns in Struktur und Ordnung. Beziehungen sind der Datenbank dabei sehr wichtig.',
    },
    {
      icon: 'img/technology/mongodb.svg',
      iconAlt: 'mongodb',
      title: 'MongoDB',
      text:
        'Damit auch unstruktierte Informationen ihren Platz finden. MongoDB ist nicht wählerisch und speichert alles!',
    },
    {
      icon: 'img/technology/elasticsearch.svg',
      iconAlt: 'elasticsearch',
      title: 'Elasticsearch',
      text:
        'Elasticsearch findet in noch so grossen Datenmengen die relevanten Resultate. Datenmessies können wieder aufatmen.',
    },
    {
      icon: 'img/technology/docker.svg',
      iconAlt: 'docker',
      title: 'Docker',
      text: 'Jede Anwendung braucht klare Grenzen. Docker hilft uns dabei und regelt die Softwareverteilung.',
    },
    {
      icon: 'img/technology/kubernetes.svg',
      iconAlt: 'kubernetes',
      title: 'Kubernetes',
      text:
        'Der Chef in unserer IT Infrastruktur, welcher den Laden schmeisst und sagt wo es lang geht. In der Cloud sowie bei unsere Kunden Vorort.',
    },
    {
      icon: 'img/technology/gitlab.svg',
      iconAlt: 'gitlab',
      title: 'Gitlab',
      text:
        'Verwaltet unseren Sourcecode und produziert daraus Software. Die Landkarte und der Compass in unserer Projekten, zeigt uns wohin es geht.',
    },
    {
      icon: 'img/technology/prometheus.svg',
      iconAlt: 'prometheus',
      title: 'Prometheus',
      text:
        'Jemand der uns erinnert, wann es mal nicht rund läuft. Hält stehts Kontakt mit den Entwicklern und (fast) Teil der Familie.',
    },
    {
      icon: 'img/technology/kibana.svg',
      iconAlt: 'kibana',
      title: 'Kibana',
      text: 'Unser Verbündeter im Kampf gegen die kniffligen Bugs. Zeichnet die Lebenszeichen aller Anwendungen auf.',
    },
    {
      icon: 'img/technology/sentry.svg',
      iconAlt: 'sentry',
      title: 'Sentry',
      text: 'Ein Insider, welcher die Probleme unserer Anwendung vor den Awender erkennt.',
    },
    {
      icon: 'img/technology/digitalocean.svg',
      iconAlt: 'digitalocean',
      title: 'Digitalocean',
      text: 'Die Platform für Infrastruktur in der Cloud mit kleinem Budget und viel Herz. ',
    },
    {
      icon: 'img/technology/gcloud.svg',
      iconAlt: 'google cloud',
      title: 'Google Cloud',
      text: 'Die Platform für Infrastruktur in der Cloud mit Standorten in der Schweiz',
    },
    {
      icon: 'img/technology/azure.svg',
      iconAlt: 'azure',
      title: 'Azure Cloud',
      text: 'Die Platform für Infrastruktur in der Cloud verknüpft mit ihrem Office Paket',
    },
  ]
</script>

<div class="bg-blue-triarc text-white" id="technology">
  <div class="max-w-screen-xl mx-auto py-12 px-4 text-center sm:px-6 lg:px-8 lg:py-24">
    <div class="space-y-8 sm:space-y-12">
      <div class="space-y-5 sm:mx-auto sm:max-w-xl sm:space-y-4 lg:max-w-5xl">
        <h2 class="text-3xl leading-9 font-extrabold tracking-tight sm:text-4xl">Unsere Technologien</h2>
        <p class="text-xl leading-7 text-gray-200">
          Die Technologie die wir einsetzen sind vielfältig und haben alle das Ziel, unsere Projekte mit dem gewissen
          etwas zu verleihen. Damit unsere Projekte stehts aktuell bleiben und wir ein einzigartiges Benutzererlebniss
          anbieten können, bleiben wir stehts auf dem aktuellen Stand der Technik.
        </p>
      </div>
      <div class="grid self-center mt-8 grid-cols-1 gap-6 gap-y-6 md:grid-cols-2 lg:grid-cols-3">
        {#each technologies as technology}
          <div class="flex items-center">
            <img class="w-12" src={technology.icon} alt={technology.iconAlt} />
            <div class="text-left ml-4">
              <div class="text-xl underline">{technology.title}</div>
              <div class="text-gray-100">
                {technology.text}
              </div>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
</div>

<style>
  .grayscale {
    filter: grayscale(100%);
    transition-duration: 0.3s;
    transition-timing-function: ease-out;
    transition-property: filter;
  }
  .grayscale:hover {
    filter: none;
  }
</style>
