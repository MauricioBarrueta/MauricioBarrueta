
  <button onclick="langChange('es')">Español</button>
  <button onclick="langChange('en')">English</button>
  <h2 style="text-align: center;" data-es="Hola" data-en="Hi">🖖🙂&nbsp; Mi nombre es Edgar Mauricio Barrueta Aguirre</h2>

  <p style="font-size: 24px;">Desarrollador web front end egresado como ingeniero en Tecnologías de la Información y Comunicación (TIC) 👨‍🎓</p>

  <p style="text-align: center">
    <a href="https://skillicons.dev">
      <img src="https://skillicons.dev/icons?i=js,ts,java,c,vim" />
    </a>
  </p>

  <script src="https://code.jquery.com/jquery-3.7.1.js" integrity="sha256-eKhayi8LEQwp4NKxN+CfCh+3qOVUtJn3QNZ0TciWLP4=" crossorigin="anonymous"></script>
  <script>
    /* Traduce el contenido de toda la página a inglés o español */
    var currLang //* Almacena el idioma actual de la página
    const langChange = (lang) => {
      currLang = lang
      $(`[data-${lang}]`).text(function () { return $(this).data(lang) })      
    }
    langChange()
    $('.lang-btn').click(function () {
      langChange($(this).data('lang'))
      langChangeAlert()
    })
  </script>

