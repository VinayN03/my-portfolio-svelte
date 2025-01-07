<script lang="ts">


const techStack = [
    {
        title: "Python",
        stack: ['virtualenv', 'flask', 'gunicorn', 'waitress', 'flask-restful', 'fastai',
        'jupyter notebook', 'streamlit', 'pdftotext', 'pyhtml2pdf', 'beautifulsoup', 'hocrtools', 'mmocr',
        'paddle-ocr', 'pytesseract', 'google-cloud-vision', 'google-vision-ocr', 'amazon textract',
        'pymysql', 'sqlalchemy', 'oracle-client']
    },
    {
        title: "ML, DL & NLP",
        stack: ['pandas', 'numpy', 'scikit-learn', 'seaborn', 'matplotlib', 'opencv',
        'pytorch', 'tensorflow', 'keras',
         'nltk', 'spacy'
        ]
    },
    {
        title: "Generative AI",
        stack: ['transformers', 'openAI', 'pandasAI', 'Ollama', 'DSPy', 'langchain',
                'huggingface', 'LLAMA2', 'LLAMA3', 'Mistral']
    },
    {
        title: "AWS & Others",
        stack: ['EC2', 'Lambda', 'S3', 'Cloudwatch', "Svelte", "TagUI", "putty", "winscp", "docker",
         "postman", "ubuntu", "cuda", "cudnn"]
    },
]
</script>

<div class="tech-stack">
<div class="default-margin mt-m mb-l">
    <h3>Tech Stack</h3>
    <div class="underscore"></div>
    <div>
    {#each techStack as category}
    <div class="ts-title">{category.title}</div>
    <div class="tech-stack-list mt-xs">
    {#each category.stack as item}
    <p>{item}</p>
    {/each}
</div>
    {/each}
    </div>

</div>
</div>

<style>
    .tech-stack {
        background-color: #fbfbfb;
        width: 100%;
        padding-top: 30px;
        padding-bottom: 30px;
        
    }

    .tech-stack-list {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        align-items: normal;
    }

    .ts-title {
        display: block;
        text-align: right;
        font-size: 14px;
        font-weight: bold;
        margin-bottom: 5px;
        padding-bottom: 0px;
        margin-top: 5px;
    }

    .tech-stack p {
        margin-right: 5px;
        border: 1px solid #f0eded;
        border-radius: 5px;
        padding: 5px 10px;
    }
</style>