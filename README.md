# Document-Term-Frequency

1. Text Preprocessing
Tokenizing and preparing a sample corpus of documents.
This step involves breaking down raw text into smaller units (tokens), such as words or phrases, to make them suitable for analysis.

2. Term Frequency Analysis
Raw Term Frequency:
Counts the occurrences of each term (word) in a document.
Provides a simple measure of how often a word appears.

Normalized Term Frequency:
Adjusts the term frequencies by dividing by the total number of terms in the document.
This ensures the term frequencies are proportional and comparable across documents.

3. TF-IDF Calculation
Absolute TF-IDF:
Combines term frequency (TF) and inverse document frequency (IDF) to assign a score to each term.
Highlights terms that are frequent in a document but rare across the entire corpus.
Normalized TF-IDF:
Scales TF-IDF scores using L1 or L2 normalization:
L1 Normalization: Scales scores so that the sum of all term scores in a document equals 1.
L2 Normalization: Scales scores so that the square root of the sum of squared scores equals 1.

4. Implementation
The analysis leverages tools from the scikit-learn library:
CountVectorizer: For extracting raw term frequency from the corpus.
TfidfVectorizer: For calculating absolute and normalized TF-IDF scores.
