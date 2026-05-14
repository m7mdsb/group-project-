/* المتغيرات الأساسية المستوحاة من ألوان التراث */
:root {
    --primary-color: #8b4513;   /* البني الخشبي */
    --secondary-color: #fdfaf3; /* اللون الكريمي */
    --accent-color: #c19a6b;    /* لون الرمال */
    --text-color: #2d241e;      /* البني الداكن للنصوص */
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Tajawal', sans-serif;
    background-color: var(--secondary-color);
    color: var(--text-color);
    line-height: 1.8;
}

/* الهيدر مع صورة خلفية */
header {
    background-image: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                      url('https://images.unsplash.com/photo-1512621776951-a57141f2eefd?auto=format&fit=crop&q=80');
    background-size: cover;
    background-position: center;
    height: 70vh;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    text-align: center;
}

header h1 {
    font-family: 'Amiri', serif;
    font-size: 4rem;
    margin-bottom: 10px;
    text-shadow: 2px 2px 10px rgba(0,0,0,0.5);
}

/* التنسيق العام للحاويات */
.container {
    max-width: 1100px;
    margin: 50px auto;
    padding: 0 20px;
}

.section-title {
    text-align: center;
    font-size: 2.5rem;
    color: var(--primary-color);
    margin-bottom: 40px;
    border-bottom: 3px solid var(--accent-color);
    display: inline-block;
    width: 100%;
}

/* نظام الشبكة (Grid) للبطاقات */
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.card {
    background: white;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 10px 20px rgba(0,0,0,0.05);
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-10px);
}

.card-img {
    height: 200px;
    background-size: cover;
    background-position: center;
}

.card-content {
    padding: 20px;
}

.card-content h3 {
    color: var(--primary-color);
    margin-bottom: 10px;
}

footer {
    background: var(--primary-color);
    color: white;
    text-align: center;
    padding: 30px 0;
    margin-top: 50px;
}
