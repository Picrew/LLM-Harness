# Agent Harness Engineering: A Survey

Companion page to *Agent Harness Engineering: A Survey*. The site introduces the ETCLOVG
seven-layer taxonomy and points to the public catalog of agent-harness projects
maintained at [Awesome-Agent-Harness](https://github.com/Picrew/awesome-agent-harness).

- **Live page:** <https://picrew.github.io/LLM-Harness/>
- **Paper (OpenReview):** <https://openreview.net/forum?id=eONq7FdiHa>
- **Catalog:** <https://github.com/Picrew/awesome-agent-harness>
- **Dataset (HuggingFace):** <https://huggingface.co/datasets/ChenLiu1996/Agent-Harness-Engineering>

## What is in this repository

```
.
├── docs/                 GitHub Pages site
│   ├── index.html        single-page project page
│   ├── assets/
│   │   ├── css/          stylesheet
│   │   └── figs/         figures shared with the paper
│   └── .nojekyll
├── LICENSE
├── README.md
└── .gitignore
```

The site is deliberately dependency-free: plain HTML and CSS with a small piece of
inline JavaScript for the copy-BibTeX button. Any static server can preview it.

## Run locally

```bash
python3 -m http.server 8080 --directory docs
# or
npx serve docs
```

Then open <http://localhost:8080>.

## Deploy on GitHub Pages

1. Push this repository to GitHub.
2. Open **Settings → Pages**.
3. Set **Source = Deploy from a branch**, **Branch = `main`**, **Folder = `/docs`**.

## Reference template

The page layout follows the conventions of common academic project pages (centered
hero, abstract, taxonomy figure, citation block). The visual treatment is hand-rolled
rather than templated, but it is in the same spirit as the
[Nerfies](https://github.com/nerfies/nerfies.github.io) project-page family.

## Citation

```bibtex
@misc{li2026agentharness,
  title  = {Agent Harness Engineering: A Survey},
  author = {Junjie Li and Xi Xiao and Yunbei Zhang and Chen Liu and
            Lin Zhao and Xiaoying Liao and Yingrui Ji and Janet Wang and
            Jianyang Gu and Yingqiang Ge and Weijie Xu and Xi Fang and
            Xiang Xu and Tianchen Zhao and Youngeun Kim and
            Tianyang Wang and Jihun Hamm and Smita Krishnaswamy and
            Jun Huan and Chandan K. Reddy},
  year   = {2026},
  note   = {Preprint}
}
```

## License

The contents of `docs/` are released under
[CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/); code in this repository
is released under the [MIT License](LICENSE).
