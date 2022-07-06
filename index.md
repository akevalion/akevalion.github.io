<main id="main-content" style="scroll-margin-top: 5rem;">
<div class="container-xl px-3 px-md-6 my-4">
<div class="Box-sc-1gh2r6s-0 sc-bczRLJ  fDvZIH">
<div class="Box-sc-1gh2r6s-0 iYYqoc">
<div class="d-flex flex-items-baseline flex-justify-between">
<h1 class="border-bottom-0">Quickstart for GitHub Actions</h1>
</div></div>
<div class="Box-sc-1gh2r6s-0 sc-gsnTZi dsDXDh fFuyXS border-bottom border-xl-0 pb-4 mb-5 pb-xl-0 mb-xl-0">
<h2 id="in-this-article" class="Heading-sc-1irtotl-0 jDbaZj mb-1">
<a rel="" href="/actions/quickstart#in-this-article">En este artículo</a>
</h2>
<div class="List__StyledList-sc-1x7olzq-0 gQuVvX">
<div class="Group__StyledGroup-sc-cnw2p9-0 kFAJDP">
<ul>
<li tabindex="-1" class="Item__StyledItem-sc-yeql7o-2 jggHqs">
<div class="Item__DividedContent-sc-yeql7o-0 eBArJY"><div class="Item__MainContent-sc-yeql7o-1 bzHypO" style="--main-content-flex-direction:row;"><div class="lh-condensed d-block width-full"><a class="d-block width-auto" href="#introduction">Introduction</a></div></div></div></li></ul><ul><li tabindex="-1" class="Item__StyledItem-sc-yeql7o-2 jggHqs"><div class="Item__DividedContent-sc-yeql7o-0 eBArJY"><div class="Item__MainContent-sc-yeql7o-1 bzHypO" style="--main-content-flex-direction:row;"><div class="lh-condensed d-block width-full"><a class="d-block width-auto" href="#creating-your-first-workflow">Creating your first workflow</a></div></div></div></li></ul><ul><li tabindex="-1" class="Item__StyledItem-sc-yeql7o-2 jggHqs"><div class="Item__DividedContent-sc-yeql7o-0 eBArJY"><div class="Item__MainContent-sc-yeql7o-1 bzHypO" style="--main-content-flex-direction:row;"><div class="lh-condensed d-block width-full"><a class="d-block width-auto" href="#viewing-your-workflow-results">Viewing your workflow results</a></div></div></div></li></ul><ul><li tabindex="-1" class="Item__StyledItem-sc-yeql7o-2 jggHqs"><div class="Item__DividedContent-sc-yeql7o-0 eBArJY"><div class="Item__MainContent-sc-yeql7o-1 bzHypO" style="--main-content-flex-direction:row;"><div class="lh-condensed d-block width-full"><a class="d-block width-auto" href="#more-starter-workflows">More starter workflows</a></div></div></div></li></ul><ul><li tabindex="-1" class="Item__StyledItem-sc-yeql7o-2 jggHqs"><div class="Item__DividedContent-sc-yeql7o-0 eBArJY"><div class="Item__MainContent-sc-yeql7o-1 bzHypO" style="--main-content-flex-direction:row;"><div class="lh-condensed d-block width-full"><a class="d-block width-auto" href="#more-complex-examples">More complex examples</a></div></div></div></li></ul><ul><li tabindex="-1" class="Item__StyledItem-sc-yeql7o-2 jggHqs"><div class="Item__DividedContent-sc-yeql7o-0 eBArJY"><div class="Item__MainContent-sc-yeql7o-1 bzHypO" style="--main-content-flex-direction:row;"><div class="lh-condensed d-block width-full"><a class="d-block width-auto" href="#next-steps">Next steps</a></div></div></div></li></ul></div></div></div><div class="Box-sc-1gh2r6s-0 gpLjoq"><div class="f2 color-fg-muted mb-3 Lead_container__g1kT8" data-testid="lead" data-search="lead"><p>Try out the features of GitHub Actions in 5 minutes or less.</p></div></div><div data-search="article-body" class="Box-sc-1gh2r6s-0 fWkkBJ"><div id="article-contents"><div class="MarkdownContent_markdownBody__gRgTE markdown-body"><!-- 2BB13A4A-041C-4064-9A7A-B482C5BC964F -->
<h2 id="introduction"><a aria-hidden="" tabindex="-1" class="doctocat-link" href="#introduction"><svg aria-hidden="" role="img" class="octicon-link" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:middle"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Introduction</h2>
<p>You only need a GitHub repository to create and run a GitHub Actions workflow. In this guide, you'll add a workflow that demonstrates some of the essential features of GitHub Actions. </p>
<p>The following example shows you how GitHub Actions jobs can be automatically triggered, where they run, and how they can interact with the code in your repository.</p>
<h2 id="creating-your-first-workflow"><a aria-hidden="" tabindex="-1" class="doctocat-link" href="#creating-your-first-workflow"><svg aria-hidden="" role="img" class="octicon-link" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:middle"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Creating your first workflow</h2>
<ol>
<li>
<p>Create a <code>.github/workflows</code> directory in  your repository on GitHub if this directory does not already exist.</p>
</li>
<li>
<p>In the <code>.github/workflows</code> directory, create a file named <code>github-actions-demo.yml</code>. For more information, see "<a href="/es/github/managing-files-in-a-repository/creating-new-files">Creating new files</a>."</p>
</li>
<li>
<p>Copy the following YAML contents into the <code>github-actions-demo.yml</code> file:</p>
<div class="code-extra"><header class="d-flex flex-items-center flex-justify-between p-2 text-small rounded-top-1 border"><span>YAML</span><button class="js-btn-copy btn btn-sm tooltipped tooltipped-nw" data-clipboard-text="name: GitHub Actions Demo
on: [push]
jobs:
  Explore-GitHub-Actions:
    runs-on: ubuntu-latest
    steps:
      - run: echo &quot;🎉 The job was automatically triggered by a ${{ github.event_name }} event.&quot;
      - run: echo &quot;🐧 This job is now running on a ${{ runner.os }} server hosted by GitHub!&quot;
      - run: echo &quot;🔎 The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}.&quot;
      - name: Check out repository code
        uses: actions/checkout@v3
      - run: echo &quot;💡 The ${{ github.repository }} repository has been cloned to the runner.&quot;
      - run: echo &quot;🖥️ The workflow is now ready to test your code on the runner.&quot;
      - name: List files in the repository
        run: |
          ls ${{ github.workspace }}
      - run: echo &quot;🍏 This job's status is ${{ job.status }}.&quot;
" aria-label="Copy code to clipboard"><svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-copy" aria-hidden="true"><path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path></svg></button></header><pre><code class="hljs language-yaml"><span class="hljs-attr">name:</span> <span class="hljs-string">GitHub</span> <span class="hljs-string">Actions</span> <span class="hljs-string">Demo</span>
<span class="hljs-attr">on:</span> [<span class="hljs-string">push</span>]
<span class="hljs-attr">jobs:</span>
  <span class="hljs-attr">Explore-GitHub-Actions:</span>
    <span class="hljs-attr">runs-on:</span> <span class="hljs-string">ubuntu-latest</span>
    <span class="hljs-attr">steps:</span>
      <span class="hljs-bullet">-</span> <span class="hljs-attr">run:</span> <span class="hljs-string">echo</span> <span class="hljs-string">"🎉 The job was automatically triggered by a $<span class="hljs-template-variable">{{ github.event_name }}</span> event."</span>
      <span class="hljs-bullet">-</span> <span class="hljs-attr">run:</span> <span class="hljs-string">echo</span> <span class="hljs-string">"🐧 This job is now running on a $<span class="hljs-template-variable">{{ runner.os }}</span> server hosted by GitHub!"</span>
      <span class="hljs-bullet">-</span> <span class="hljs-attr">run:</span> <span class="hljs-string">echo</span> <span class="hljs-string">"🔎 The name of your branch is $<span class="hljs-template-variable">{{ github.ref }}</span> and your repository is $<span class="hljs-template-variable">{{ github.repository }}</span>."</span>
      <span class="hljs-bullet">-</span> <span class="hljs-attr">name:</span> <span class="hljs-string">Check</span> <span class="hljs-string">out</span> <span class="hljs-string">repository</span> <span class="hljs-string">code</span>
        <span class="hljs-attr">uses:</span> <span class="hljs-string">actions/checkout@v3</span>
      <span class="hljs-bullet">-</span> <span class="hljs-attr">run:</span> <span class="hljs-string">echo</span> <span class="hljs-string">"💡 The $<span class="hljs-template-variable">{{ github.repository }}</span> repository has been cloned to the runner."</span>
      <span class="hljs-bullet">-</span> <span class="hljs-attr">run:</span> <span class="hljs-string">echo</span> <span class="hljs-string">"🖥️ The workflow is now ready to test your code on the runner."</span>
      <span class="hljs-bullet">-</span> <span class="hljs-attr">name:</span> <span class="hljs-string">List</span> <span class="hljs-string">files</span> <span class="hljs-string">in</span> <span class="hljs-string">the</span> <span class="hljs-string">repository</span>
        <span class="hljs-attr">run:</span> <span class="hljs-string">|
          ls ${{ github.workspace }}
</span>      <span class="hljs-bullet">-</span> <span class="hljs-attr">run:</span> <span class="hljs-string">echo</span> <span class="hljs-string">"🍏 This job's status is $<span class="hljs-template-variable">{{ job.status }}</span>."</span>
</code></pre></div>
</li>
<li>
<p>Scroll to the bottom of the page and select <strong>Create a new branch for this commit and start a pull request</strong>. Then, to create a pull request, click <strong>Propose new file</strong>.
<span class="procedural-image-wrapper"><img src="/assets/cb-67235/images/help/repository/actions-quickstart-commit-new-file.png" alt="Commit workflow file"></span></p>
</li>
</ol>
<p>Committing the workflow file to a branch in your repository triggers the <code>push</code> event and runs your workflow.</p>
<h2 id="viewing-your-workflow-results"><a aria-hidden="" tabindex="-1" class="doctocat-link" href="#viewing-your-workflow-results"><svg aria-hidden="" role="img" class="octicon-link" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:middle"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Viewing your workflow results</h2>
<ol>
<li>
<p>En GitHub.com, visita la página principal del repositorio.</p>
</li>
<li>
<p>Debajo de tu nombre de repositorio, haz clic en <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-play" aria-label="The Play icon" role="img"><path fill-rule="evenodd" d="M1.5 8a6.5 6.5 0 1113 0 6.5 6.5 0 01-13 0zM8 0a8 8 0 100 16A8 8 0 008 0zM6.379 5.227A.25.25 0 006 5.442v5.117a.25.25 0 00.379.214l4.264-2.559a.25.25 0 000-.428L6.379 5.227z"></path></svg> <strong>Acciones</strong>. <span class="procedural-image-wrapper"><img src="/assets/cb-13492/images/help/repository/actions-tab.png" alt="Pestaña de acciones en la navegación del repositorio principal"></span></p>
</li>
<li>
<p>In the left sidebar, click the workflow you want to see.</p>
<p><span class="procedural-image-wrapper"><img src="/assets/cb-55861/images/help/repository/actions-quickstart-workflow-sidebar.png" alt="Workflow list in left sidebar"></span></p>
</li>
<li>
<p>From the list of workflow runs, click the name of the run you want to see.</p>
<p><span class="procedural-image-wrapper"><img src="/assets/cb-57054/images/help/repository/actions-quickstart-run-name.png" alt="Name of workflow run"></span></p>
</li>
<li>
<p>Under <strong>Jobs</strong> , click the <strong>Explore-GitHub-Actions</strong> job.</p>
<p><span class="procedural-image-wrapper"><img src="/assets/cb-46973/images/help/repository/actions-quickstart-job.png" alt="Locate job"></span></p>
</li>
<li>
<p>The log shows you how each of the steps was processed. Expand any of the steps to view its details.</p>
<p><span class="procedural-image-wrapper"><img src="/assets/cb-102539/images/help/repository/actions-quickstart-logs.png" alt="Example workflow results"></span></p>
<p>For example, you can see the list of files in your repository:
<span class="procedural-image-wrapper"><img src="/assets/cb-39565/images/help/repository/actions-quickstart-log-detail.png" alt="Example action detail"></span></p>
</li>
</ol>
<h2 id="more-starter-workflows"><a aria-hidden="" tabindex="-1" class="doctocat-link" href="#more-starter-workflows"><svg aria-hidden="" role="img" class="octicon-link" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:middle"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>More starter workflows</h2>
<p>GitHub Proporciona un flujo de trabajo preconfigurado que puedes personalizar para crear tu propio flujo de trabajo de integración contínua. GitHub analiza tu código y te muestra el flujo de trabajo inicial de IC que podría ser útil para tu repositorio. Por ejemplo, si tu repositorio contiene un código Node.js, verás sugerencias para los proyectos de Node.js. Puedes utilizar el flujo de trabajo inicial como un lugar para comenzar a crear tu flujo de trabajo personalizado o utilizarlo tal cual.</p>
<p>Puedes buscar la lista completa de flujos de trabajo iniciales en el repositorio <a href="https://github.com/actions/starter-workflows">actions/starter-workflows</a>.</p>
<h2 id="more-complex-examples"><a aria-hidden="" tabindex="-1" class="doctocat-link" href="#more-complex-examples"><svg aria-hidden="" role="img" class="octicon-link" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:middle"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>More complex examples</h2>
<p>For examples that demonstrate more complex features of GitHub Actions, see "<a href="/es/actions/examples">Examples</a>." You can see detailed examples that explain how to test your code on a runner, access the GitHub CLI, and use advanced features such as concurrency and test matrices.</p>
<h2 id="next-steps"><a aria-hidden="" tabindex="-1" class="doctocat-link" href="#next-steps"><svg aria-hidden="" role="img" class="octicon-link" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" style="display:inline-block;user-select:none;vertical-align:middle"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Next steps</h2>
<p>The example workflow you just added runs each time code is pushed to the branch, and shows you how GitHub Actions can work with the contents of your repository. But this is only the beginning of what you can do with GitHub Actions:</p>
<ul>
<li>Your repository can contain multiple workflows that trigger different jobs based on different events. </li>
<li>You can use a workflow to install software testing apps and have them automatically test your code on GitHub's runners. </li>
</ul>
<p>GitHub Actions can help you automate nearly every aspect of your application development processes. Ready to get started? Here are some helpful resources for taking your next steps with GitHub Actions:</p>
<ul>
<li>"<a href="/es/actions/learn-github-actions">Learn GitHub Actions</a>" for an in-depth tutorial.</li>
</ul></div></div></div></div></div></main>