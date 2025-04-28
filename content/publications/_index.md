---
title: ""
---

We generally publish our research in top robotics venues<br> <i>(e.g., ICRA, IROS, Robotics & Automation Letters, Human-Robot Interaction)</i>.

<p>We aim to make our research broadly available by hosting publication pre-prints to Arxiv. You can find an automatically generated list of pre-prints <u>below</u>.</p>

<p> You can also find an up-to-date list of publications on <a href="https://scholar.google.com/citations?user=pvBZ1KAAAAAJ&hl=en"><b>Prof. Hagenow's google scholar</b></a> and please also subscribe to the <a href="https://youtube.com/@hagenowrobotics?si=_xWaS375kVWyoXUj"><b>RT² Lab Youtube Channel</b></a> for new research videos</a>. </p>

<div id="arxivfeed" class="arxiv-wrapper"></div>

<style>
.arxiv-wrapper {
  max-width: 800px;
  margin: 2rem auto;
  padding: 1rem;
  /* background-color: #f9f9f9; */
  border-left: 4px solid #8E1E24;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
  font-family: sans-serif;
  font-size: 0.95rem;
  line-height: 1.5;
}
.arxiv-wrapper a {
  color: #8E1E24;
  text-decoration: none;
}
.arxiv-wrapper a:hover {
  text-decoration: underline;
}
.arxiv-wrapper .arxivfeed {
  width: 100% !important; /* override inline width from the script */
}

/* Make arXiv URLs black */
.arxivfeed a[href*="arxiv.org/abs"] {
  color: black !important;
  text-decoration: none;
}

/* Add spacing before [html pdf] links */
.arxivfeed b + br {
  display: none;
}
.arxivfeed b + a[href*="html"]::before {
  content: "\A";
  white-space: pre;
  display: block;
  margin-top: 0.2rem;
}

/* Optional: reduce bottom margin between entries */
.arxivfeed > div {
  margin-bottom: 1.5rem;
}

</style>


<script>
  var arxiv_authorid = "hagenow_m_1";
  var arxiv_max_entries = 8;
  var arxiv_format = "arxiv";
  var arxiv_includeTitle = 0;
  var arxiv_includeSummary = 0;
</script>
<script src="https://arxiv.org/js/myarticles.js" defer></script>



<script>
function removeSpecificArxivAbsLink() {
  const targetText = "arxiv.org"; // ← part of the link text you want to match
  const arxivLinks = document.querySelectorAll('#arxivfeed a[href*="arxiv.org/abs"]');
  if (arxivLinks.length > 0) {
    arxivLinks.forEach(link => {
      if (link.textContent.includes(targetText)) {
        link.remove();
      }
    });
  } else {
    setTimeout(removeSpecificArxivAbsLink, 200); // Retry if widget isn't ready
  }
}

document.addEventListener("DOMContentLoaded", function() {
  removeSpecificArxivAbsLink();
});
</script>


