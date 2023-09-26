# Borderless_Azerbaijani_Processing

### Introduction
This repository showcases a Transformer-based approach for Azerbaijani transliteration, bridging the gap between Persian and Latin scripts to facilitate seamless communication and cultural exchange, as accepted at IJCNLP-AACL 2023.

#### Abstract
Recent advancements in neural language models have revolutionized natural language understanding. However, many languages still face the risk of being left behind without the benefits of such advancements, potentially leading to their extinction. One such language is Azerbaijani in Iran, which suffers from limited digital resources and a lack of alignment between spoken and written forms. In contrast, Azerbaijani in the Republic of Azerbaijan has seen more resources and is not considered as low-resource as its Iranian counterpart. In this context, our research focuses on the computational progress made in Iranian Azerbaijani language. We propose a transliteration model that leverages an Azerbaijani parallel dataset, effectively bridging the gap between the Latin and Persian scripts. By enabling seamless communication between these two scripts, our model facilitates cultural exchange and serves as a valuable tool for transfer learning. The effectiveness of our approach surpasses traditional rule-based methods, as evidenced by the significant improvements in performance metrics. We observe a minimum 15% increase in BLEU scores and a reduction of at least 1/3 in edit distance. Furthermore, our model’s online demo is accessible at [https://azeri.parsi.ai/](https://azeri.parsi.ai/).

### Key Contributions
Our primary contributions include:
1. The creation of a parallel dataset encompassing both Iranian and Azerbaijani variants of Azerbaijani.
2. A thorough analysis of existing transliteration tools for Iranian Azerbaijani.
3. The development of a transliteration model to enhance resources for Iranian Azerbaijani.

### Results Summary
Here's a summary of our key results:

**Table 3: Performance Comparison of Transliteration Models**
| Model                   | Min. Edit Dist. d | Avg. Len. | BLEU |
|-------------------------|-------------------|-----------|------|
| Transformer (Persian-to-Latin) | 0.31 ± 0.1 | 8 | 0.94 ± 2.6 |
| Transformer (Latin-to-Persian) | 0.33 ± 0.06 | 7 | 0.94 ± 1.7 |
| polyglot | 3.56 | 8 | 0.45 |
| Azconvert | 1.12 | 8 | 0.79 |
| LSTM | 0.47 | 8 | 0.91 |

**Table 4: Out-of-Domain Comparison of Transliteration Methods**
| Model                   | Min. Edit Dist. d | Avg. Len. | BLEU |
|-------------------------|-------------------|-----------|------|
| Transformer (Persian-to-Latin) | 0.17 | 5.2 | 0.96 |
| Transformer (Latin-to-Persian) | 0.32 | 5.3 | 0.91 |
| polyglot | 2.34 | 5.2 | 0.21 |
| Azconvert | 0.64 | 5.2 | 0.83 |
| ChatGPT | 1.49 | 5.2 | 0.66 |

The comparison results in Tables 3 and 4 highlight the significant performance improvements achieved by the Transformer model compared to Azconvert rule-based and polyglot statistical methods. The trained transliteration model achieved impressive BLEU scores for both directions, despite the limited resources and calligraphy-related challenges.

### Contact
For any questions or inquiries, please feel free to reach out to us at reihane.zohrabi@gmail.com.

