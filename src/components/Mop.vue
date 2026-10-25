<template>
  <div id="mop">
    <div
      v-for="(lomda, index) in mopData"
      :key="index"
      :id="lomda.id"
      class="lomda-card"
    >
      <img :src="lomda.src" :alt="lomda.id" class="lomda-img" :id="lomda.id" />
      <p class="lomda-title">{{ lomda.title }}</p>
      <p class="lomda-text">{{ lomda.text }}</p>
      <img :src="lomda.qr" :alt="lomda.id" class="lomda-qr" :id="lomda.id" />
    </div>
  </div>
</template>

<script>
export default {
  name: "mop",
  components: {
  },
  data() {
    return {
      mopData: [
        { id: "hinuch", title: "שאלון מי אני?", text: 'פותח ל"פסטיבל מתגייסים". משחקון למלש"בים המיועדים לגיוס בחיל החינוך והנוער.', src: "./assets/mop/hinuch.png", qr: "./assets/mop/hinuch-qr.jpg" },
        {
          id: "kosher",
          title: "אתר כושר",
          text: "אתר מידע למדור כושר. מכיל בתוכו את כל המידע הרלוונטי על כושר ואימון גופני בקריית ההדרכה.",
          src: "./assets/mop/kosher.png",  qr: "./assets/mop/sport-qr.jpg"
        },
        { id: "arrestDocuments", title: "לומדת מסמכי מעצר", text: 'פותח עבור קורס חוקרי מצ"ח בבה"ד 13. הלומדה עוזרת לחיילי הקורס לתרגל מילוי מסמכי מעצר.', src: "./assets/mop/arrestDocuments.png", qr: "./assets/mop/arrest-qr.jpg" },
        { id: "learningGame", title: "משחוק בלמידה מרחוק", text: "לומדת הסבר על כלים דיגיטליים המסייעים בתכנון והעברת הדרכות או הכשרות מרחוק. פותח במהלך מלחמת עם כלביא.", src: "./assets/mop/learningGame.png", qr: "./assets/mop/game-qr.jpg" },
        { id: "cranes", title: "לומדת עגורנים", text: 'פותח עבור קורס עגורנים בבה"ד 20. נועד להעביר את החלק התאורטי של הקורס ללמידה מרחוק.', src: "./assets/mop/cranes.png", qr: "./assets/mop/cranes-qr.jpg" },
        { id: "cranes", title: "פנקס סדרי בראשית", text: 'פקלון כיס המאגד מידע חשוב על מפקדת קריית ההדרכה עבור חיילי המפקדה.', src: "./assets/mop/bereshit.png", qr: "./assets/mop/bereshit-qr.jpg" },
        { id: "cranes", title: "הכרת מטה חיל החינוך והנוער", text: 'פקלון מידע אודות מטה חיל החינוך והנוער עבור חיילי בה"ד החינוך', src: "./assets/mop/mate.png", qr: "./assets/mop/mate-qr.jpg" }
      ],
    };
  },
  methods: {
  },
};
</script>

<style scoped>
#mop {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

.lomda-card {
  height: 30rem;
  width: 21rem;
  background-color: #EDFAFF;
  border: 5px solid #B3D8F3;
  border-radius: 20px;
  text-align: center;
  margin: 1rem;
  font-family: "carmela";
  padding: 0.2rem;
}

.lomda-img {
  margin-top: 0.3rem;
  max-width: 18rem;
  border-radius: 20px;
  margin-bottom: 0rem;
  max-height: 18rem;
}

.lomda-title {
  margin-top: 0rem;
  font-size: 1.8rem;
  margin-bottom: -0.5rem;
}

.lomda-text {
  margin-top: 0rem;
  margin-bottom: 0rem;
  font-size: 1rem;
}

.lomda-qr {
  margin-top: 0rem;
  height: 5rem;
}
</style>
