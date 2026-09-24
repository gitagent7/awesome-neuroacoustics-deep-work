# Contributing to Awesome Neuroacoustics & Generative Soundscapes

Thank you for your interest in contributing to the **Awesome Neuroacoustics & Generative Soundscapes** research hub and verification benchmark!

Our objective is to maintain a rigorous, peer-reviewed, open-source repository bridging cognitive neuroscience, mathematical digital signal processing (DSP), and non-invasive cognitive enhancement tools (deep work, ADHD focus, and stage-4 restorative sleep).

We welcome contributions from neuroscientists, DSP engineers, medical researchers, audiophiles, and software developers worldwide.

---

## Code of Conduct & Scientific Integrity

To maintain academic and scientific credibility, all contributors must adhere to these foundational principles:

1. **Evidence-First Standard:** Claims regarding brainwave entrainment, auditory steady-state response (ASSR), default mode network (DMN) modulation, or slow-wave sleep must be accompanied by peer-reviewed citations.
2. **Anti-Pseudoscience Policy:** We do not accept unsubstantiated claims (e.g. "manifestation frequencies", miraculous medical cures, or unscientific mysticism).
3. **Safety & Ethical Responsibility:** All acoustic discussions must clearly identify contraindications (e.g., photosensitive or auditory epilepsy, seizure disorders, or operating heavy machinery).
4. **Professional & Inclusive Environment:** We treat every contributor with respect, regardless of background or experience level.

---

## How Can You Contribute?

You can contribute across three distinct tracks:

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                                 CONTRIBUTION TRACKS                                    │
├─────────────────────────┬───────────────────────────────┬──────────────────────────────┤
│ TRACK 1: RESEARCH       │ TRACK 2: DSP BENCHMARK        │ TRACK 3: DOCUMENTATION       │
├─────────────────────────┼───────────────────────────────┼──────────────────────────────┤
│ • Add peer-reviewed     │ • Enhance verify_audio.py     │ • Listening setup guides     │
│   journal citations     │ • Multi-taper spectral PSD    │ • Acoustic hygiene protocols │
│ • Summarize clinical    │ • Stereo phase correlation    │ • Circadian lighting & OLED  │
│   entrainment trials    │ • Loudness compliance tools   │   ergonomic guidelines       │
└─────────────────────────┴───────────────────────────────┴──────────────────────────────┘
```

---

### Track 1: Peer-Reviewed Literature Additions

If you are proposing an addition to the research bibliography in `README.md`, ensure the citation adheres to the following criteria:

* **Publication Venue:** Must be published in a recognized, peer-reviewed journal (e.g., *Nature*, *Journal of Neuroscience*, *Frontiers in Human Neuroscience*, *Journal of the Acoustical Society of America*, *Sleep*, *Brain Research Bulletin*) or an accredited academic institution whitepaper (MIT, Stanford, Harvard, etc.).
* **Citation Format:** Use APA style including author(s), publication year, article title, journal, volume/issue, and DOI / URL:
  ```markdown
  * **Author, A. A., & Author, B. B. (Year).** *Title of the study.* Journal Name, Volume(Issue), Page-Range. [DOI Link](https://doi.org/...)
  ```
* **Context Annotation:** Provide a 1–2 sentence summary explaining the practical relevance to functional acoustic entrainment (e.g., target frequency band, carrier interaction, or neural mechanism).

---

### Track 2: DSP Benchmark & Analysis Tool Enhancements (`verify_audio.py`)

We maintain a lightweight, zero-dependency (NumPy, SciPy, SoundFile only) verification benchmark to audit audio files for scientific compliance.

We welcome PRs that enhance:
* High-resolution spectral differential estimation (e.g., Thomson multi-taper PSD, Welch window optimization).
* True Peak ($dBFS$) inter-sample over-detection algorithms conforming to ITU-R BS.1770-4.
* Interaural phase coherence and cross-correlation ($IACC$) metrics.
* Isochronic amplitude modulation depth and duty cycle analyzers.

**Code Guidelines:**
* Must remain compatible with Python 3.10+.
* Avoid heavy third-party dependencies; prefer standard scientific libraries (`numpy`, `scipy`).
* Include type annotations and docstrings explaining mathematical formulas.
* Ensure code runs cross-platform (Linux, macOS, Windows).

---

### Track 3: Acoustic Hygiene & Listening Guides

Contributions that clarify optimal listening environments are encouraged:
* Calibrated headphone specifications (open-back vs. planar magnetic vs. closed-back).
* Safe decibel exposure limits (OSHA / NIOSH compliance, 35%–55% volume recommendation).
* Circadian ergonomics (OLED true-black display protocols, blue-light avoidance for nocturnal recovery).

---

## Pull Request (PR) Workflow

1. **Fork the Repository:** Create your own fork on GitHub.
2. **Create a Topic Branch:**
   ```bash
   git checkout -b feat/add-mit-gamma-citation
   # or
   git checkout -b dsp/welch-psd-optimization
   ```
3. **Commit with Clear Messages:** Follow conventional commits:
   * `docs: add 2024 sleep spindle entrainment citation`
   * `feat(dsp): add inter-sample peak detection to audio verifier`
   * `fix: correct typo in gamma frequency table`
4. **Test Your Changes:**
   * If modifying code, run `python verify_audio.py <sample.wav>` to verify functionality.
   * If modifying Markdown, preview in GitHub or a Markdown viewer to check table formatting and links.
5. **Submit Pull Request:**
   * Provide a clear description of the change, citing relevant papers or DSP improvements.
   * Ensure links are valid and active.

---

## Security & Sensitive Information

* **Never commit API keys, secrets, or `.env` files.**
* All contributions must be scrubbed of private tokens, credentials, or proprietary internal tooling references.
* To report security concerns, please contact the maintainers via the GitHub Security Advisory tab.

---

## Licensing

By contributing to this repository, you agree that your contributions will be licensed under the **MIT License**.
