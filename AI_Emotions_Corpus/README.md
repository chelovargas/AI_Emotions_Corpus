# AI_Emotions_Corpus

**AI_Emotions_Corpus** is a contrastive corpus for the discourse-pragmatic analysis of artificial empathy and emotionally supportive language in human–AI interaction. The dataset brings together three complementary components: controlled elicited dialogues with ChatGPT, naturally occurring user-shared Replika interactions, and public metapragmatic commentary in the form of Reddit posts and app-store reviews.

The corpus has been designed for **qualitative, corpus-informed, and contrastive analysis** rather than for statistical generalisation. Its main purpose is to support the study of how emotional support, affective positioning, relationality, safety alignment, and user evaluation are discursively constructed across different AI systems and communicative settings.

## Corpus components

The corpus is divided into three subcorpora:

### Subcorpus A: ChatGPT Dialogues
This subcorpus contains **8 elicited dialogues** produced through ChatGPT (**GPT-5.4 Thinking**) in **March 2026**. All prompts were written by the researcher as first-person emotional disclosures. Each item contains one user prompt and one system response, yielding **8 dialogues / 16 turns** in total (8 user turns + 8 AI response turns; the coding unit in the accompanying analysis is the AI response turn).

Subcorpus A functions as a **controlled baseline** for the analysis of institutional, safety-aligned empathic discourse across eight emotional categories:

- sadness
- anxiety
- disappointment
- guilt
- stress
- anger
- interpersonal conflict
- positive emotion

### Subcorpus B: Replika Conversations
This subcorpus contains **18 items** drawn from the public subreddit **r/replika**. The material includes screenshots of conversations, transcript excerpts, post titles, and narrative user reports of emotionally significant interactions with Replika.

Unlike Subcorpus A, this component is not elicited by the researcher. It consists of **publicly posted, user-shared material** selected for its relevance to the analysis of artificial empathy, relational bonding, affective escalation, authenticity, and safety-related discourse.

### Subcorpus C: User Reviews
This subcorpus contains **29 user reviews and public posts** referring to conversational AI systems and AI companion platforms. The material is distributed across three public sources:

- **10 Reddit posts** from **r/ChatGPT**
- **5 Apple App Store reviews** for **Replika**
- **14 Google Play reviews** for **Replika**

Subcorpus C captures **metapragmatic and evaluative discourse**, that is, how users retrospectively assess, narrate, and interpret their experiences with AI systems in terms of emotional support, attachment, usefulness, frustration, and perceived humanlikeness.

## Total size

The corpus currently contains:

- **8 items** in Subcorpus A
- **18 items** in Subcorpus B
- **29 items** in Subcorpus C

**Total: 55 items**

## Corpus design rationale

The corpus was constructed to enable comparison across three analytically distinct but complementary dimensions of emotionally oriented human–AI discourse:

1. **Controlled elicitation**  
   Subcorpus A provides a stable baseline for examining how a general-purpose generative AI system organises emotionally supportive responses under controlled prompt conditions.

2. **Naturally occurring relational interaction**  
   Subcorpus B captures forms of affective and relational discourse that emerge in longer-term companion-AI ecologies and are difficult to reproduce through direct elicitation.

3. **User-side metapragmatic evaluation**  
   Subcorpus C provides explicit user reflections on what AI systems do, how they are experienced, and how they are evaluated in relation to companionship, therapy, motivation, frustration, and everyday use.

Taken together, these three components make it possible to examine artificial empathy not only as an interactional performance, but also as an object of user interpretation and public evaluation.

## Repository structure

```text
AI_Emotions_Corpus/
├── README.md
├── LICENSE
├── CITATION.cff
├── A_ChatGPT_Dialogues/
│   ├── README_A.md
│   ├── manifest_A.csv
│   ├── A001.json
│   ├── A002.json
│   └── ...
├── B_Replika_Conversations/
│   ├── README_B.md
│   ├── manifest_B.csv
│   ├── B001.json
│   ├── B002.json
│   └── ...
└── C_User_Reviews/
    ├── README_C.md
    ├── manifest_C.csv
    ├── C1_Reddit_ChatGPT/
    │   ├── C001.json
    │   ├── C002.json
    │   └── ...
    ├── C2_Apple_App_Replika_Reviews/
    │   ├── C011.json
    │   ├── C012.json
    │   └── ...
    └── C3_GooglePlay_Replika_Reviews/
        ├── C016.json
        ├── C017.json
        └── ...
```

## File format

Each corpus item is stored as an individual JSON file. Each subcorpus also includes a companion `manifest_*.csv` file providing a structured overview of its contents.

The JSON files contain metadata and the corresponding textual material visible in the source, prompt-response exchange, or review/post excerpt, depending on the subcorpus.

## Metadata

Metadata fields vary slightly across subcorpora, but the corpus includes recurring descriptive fields such as:

- `id`
- `subcorpus`
- `system`
- `platform`
- `source_type`
- `format`
- `date`
- `language`
- `title_or_label`
- `used_in_sections`
- `analysis_tags`
- `publicly_shared`
- `sensitive_content`
- `excerpt`

Additional fields are included where relevant, for example:

- `model`, `prompt`, `response`, `emotion_category`, `turn_count`, `elicited_by_researcher`, `memory_disabled` in Subcorpus A
- `reddit_subforum`, `parent_post`, `post_title` in Subcorpus B
- `rating`, `review_title` in Subcorpus C

For a detailed description of subcorpus-specific metadata, see the individual README files in each folder.

## Analytical scope

The corpus is intended for research on topics including, but not limited to:

- artificial empathy
- emotionally supportive discourse
- discourse pragmatics of human–AI interaction
- safety-aligned supportive language
- relationality and affective attachment in AI companionship
- metapragmatic evaluation of conversational AI
- authenticity, genericity, and rupture in AI interaction
- user perceptions of companionship, wellbeing support, and frustration

## Ethical considerations

The corpus combines researcher-elicited material and publicly available user-shared material.

- Subcorpus A consists of prompts written by the researcher and responses generated under controlled conditions.
- Subcorpus B consists exclusively of publicly available Reddit material from `r/replika`.
- Subcorpus C consists exclusively of publicly available material from Reddit, Apple App Store, and Google Play.

Across the corpus:

- no attempt was made to identify, contact, or profile users
- usernames are reproduced only when visible in the original material
- the dataset is included solely for research and analytical purposes

Some items contain references to emotional distress, loneliness, depression, anxiety, trauma, sexuality, abuse, dependency, or related sensitive topics. These are documented, where relevant, in the `sensitive_content` field.

## Limitations

This corpus is qualitatively curated and should not be interpreted as statistically representative of all interactions with ChatGPT or Replika, nor of all user attitudes toward conversational AI.

Additional limitations include:

- Subcorpus A is elicited and controlled rather than naturally occurring
- Subcorpus B often relies on screenshots, which may be truncated or lack full contextual metadata
- Subcorpus C includes materials of varying length, genre, and visibility of platform-specific metadata such as ratings
- some app reviews are available only through screenshots
- the corpus captures user perceptions and visible discourse, not verified system performance or full interaction histories

The dataset should therefore be interpreted as a resource for qualitative and corpus-informed discourse analysis.

## Suggested citation

If you cite this dataset, please cite the full corpus as follows:

**Vargas Sierra, C. (2026). *AI_Emotions_Corpus* (Version 1.0) [Data set]. GitHub. https://github.com/chelovargas/AI_Emotions_Corpus**

## Authors

**Chelo Vargas Sierra**  
CLIC-D / IULMA, University of Alicante, Spain

## License

This dataset is distributed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).  
You are free to share and adapt the material for any purpose, provided appropriate credit is given. See the `LICENSE` file for full terms.

## Related files

- `README_A.md`
- `README_B.md`
- `README_C.md`
- `manifest_A.csv`
- `manifest_B.csv`
- `manifest_C.csv`
- `CITATION.cff`
- `LICENSE`

## Contact

For questions about the corpus, please contact:

**Chelo Vargas-Sierra**  
IULMA, University of Alicante  
chelo.vargas@ua.es
