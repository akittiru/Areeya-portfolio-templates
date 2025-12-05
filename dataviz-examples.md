| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Data visualization examples

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>OECD Debt to GDP Ratios (1995–2019)</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      margin: 0;
      padding: 2rem 1rem 3rem;
      max-width: 960px;
      margin-inline: auto;
      line-height: 1.5;
    }
    h1 {
      text-align: center;
    }
    .viz-container {
      margin: 2rem 0 3rem;
    }
  </style>
</head>

<body>
  <h1>OECD Debt to GDP Ratios (1995–2019)</h1>

  <section class="viz-container">
    <div class="tableauPlaceholder" id="vizOECDDebt" style="position:relative">
      <noscript>
        <a href="#">
          <img
            alt="OECD Debt to GDP Ratios By Countries between 1995–2019"
            src="https://public.tableau.com/static/images/OE/OECD-DebttoGDPratios/OECD2/1.png"
            style="border:none"
          />
        </a>
      </noscript>

      <object class="tableauViz" style="display:none;">
        <param name="host_url" value="https%3A%2F%2Fpublic.tableau.com%2F" />
        <param name="embed_code_version" value="3" />
        <param name="site_root" value="" />
        <param name="name" value="OECD-DebttoGDPratios/OECD2" />
        <param name="tabs" value="no" />
        <param name="toolbar" value="yes" />
        <param name="static_image" value="https://public.tableau.com/static/images/OE/OECD-DebttoGDPratios/OECD2/1.png" />
        <param name="animate_transition" value="yes" />
        <param name="display_static_image" value="yes" />
        <param name="display_spinner" value="yes" />
        <param name="display_overlay" value="yes" />
        <param name="display_count" value="yes" />
        <param name="language" value="en-US" />
      </object>
    </div>
  </section>

  <!-- Load Tableau JS + initialize -->
  <script type="text/javascript">
    function initViz(divId) {
      var divElement = document.getElementById(divId);
      var vizElement = divElement.getElementsByTagName('object')[0];
      if (!vizElement) return;

      vizElement.style.width = '100%';
      vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
    }

    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    scriptElement.onload = function () {
      initViz('vizOECDDebt');
    };
    document.body.appendChild(scriptElement);

    window.addEventListener('resize', function () {
      initViz('vizOECDDebt');
    });
  </script>

</body>
</html>
