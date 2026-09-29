# Master Data Atlas

Single-file HTML page published as a Claude Artifact (JSON model in the page,
generated tabs, inspector, BPMN 2.0 export, automated checks).

| Project | Purpose | Version | Artifact | Source |
|---|---|---|---|---|
| Master Data Atlas | Learning project: master data reference model | v5 | https://claude.ai/artifact/RQwdyLoD7o17zoTmM1Cx9n | [reference-model/](reference-model/) |

Both artifacts are private to the owner until shared from the page's Share menu. All companies and figures are fictional.

GitHub Pages (Ask does not work outside the Claude viewer):

- https://garniebolling-git.github.io/temp_to_learn/reference-model/



## Master Data Atlas tabs
Start here · Network · Process (BPMN 2.0) · Catalogue · DQ rules · Regulation · Current state · Maturity ·
Value case (USD) · Roadmap · How it's built. Details: [reference-model/README.md](reference-model/README.md).

## Repository layout

```

reference-model/index.html   Master Data Atlas page
reference-model/README.md    atlas data model
tests/check.js               automated checks for the page (npm test runs them)
docs/roadmap.md              what is built, what is next
docs/decisions.md            decisions and reasons
docs/original-artifact-analysis.md   how the reference artifact was built
CHANGELOG.md                 each version with its published artifact version
CLAUDE.md                    instructions Claude Code reads at the start of every session
```

## Run the checks

```
npm install
npm test
```

Data cross-references resolve, the script parses, every tab renders at desktop
and phone width without errors, and each BPMN export is valid. Screenshots go to `tests/out/<page>/`.
