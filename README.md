<!DOCTYPE html>
<html>
<head>
    <title>Meus Repositórios</title>
  <div id="cabecalho">
  <!---<img style="display: inline-block;" height="180em" src="https://github-readme-stats.vercel.app/api?username=ShadeGarden&theme=yeblu&show_icons=true&count_private=true&include_all_commits=true&hide=contribs" />--->
  <img alt="rafa-js" height="30" width="40" src="https://camo.githubusercontent.com/e9141be13e6bea8c50af6d48f64700246faed666040ead23e74d4fc27bf411e3/68747470733a2f2f696d672e69636f6e73382e636f6d2f666c75656e742f34382f3030303030302f76697375616c2d73747564696f2d636f64652d323031392e706e67">
  <img alt="rafa-js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img alt="rafa-js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img alt="rafa-js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg"><br/><br/>
</div>
</head>
<body>
    <h1>Meus Repositórios no GitHub</h1>
    <ul id="repository-list"></ul>
    <script>
         const username = "ShadeGarden";
          fetch(`https://api.github.com/users/${username}/repos`)
            .then(response => response.json())
            .then(data => {
                const repositoryList = document.getElementById("repository-list");
                data.forEach(repo => {
                    const listItem = document.createElement("li");
                    const link = document.createElement("a");
                    link.href = repo.html_url;
                    link.textContent = repo.name;
                    listItem.appendChild(link);
                    repositoryList.appendChild(listItem);
                });
            })
            .catch(error => console.error(error));
    </script>
  <div style="text-align: center;">
  <img alt="Programador" height="360" width="480" src="https://github.com/kazuyabr/kazuyabr/blob/main/programador.gif">
</div>
</body>
</html>



