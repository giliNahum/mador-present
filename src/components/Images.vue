<template>
  <div id="images">
    <div class="image-card" v-for="(img, i) in data" :key="i">
      <img :src="img.src" :alt="img.alt" class="image-png" />
      <p class="img-text">{{ img.text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "images",
  components: {},
  data() {
    return {
      data: [
        {
          text: 'טקס סיום הכשרות יסוד בה"ד חינוך - 20.7.25 ',
          src: "./assets/images/endHinuchYesod1.jpg",
          alt: "endHinuchYesod1",
        },
        {
          text: 'טקס סיום הכשרות יסוד בה"ד חינוך - 20.7.25 ',
          src: "./assets/images/endHinuchYesod2.jpg",
          alt: "endHinuchYesod2",
        },
        {
          text: 'טקס סיום הכשרות יסוד בה"ד חינוך - 20.7.25 ',
          src: "./assets/images/endHinuchYesod3.jpg",
          alt: "endHinuchYesod3",
        },
        {
          text: 'טקס סיום הכשרות יסוד בה"ד חינוך - 20.7.25 ',
          src: "./assets/images/endHinuchYesod4.jpg",
          alt: "endHinuchYesod4",
        },
        {
            text: 'אימון קרב מגע סיירות - 17.2.25',
            src: "./assets/images/kravMaga.jpg",
            alt: "kravMaga",
        },
        {
            text: 'אימון קרב מגע סיירות - 17.2.25',
            src: "./assets/images/kravMaga1.jpg",
            alt: "kravMaga1",
        },
        {
            text: 'אימון קרב מגע סיירות - 17.2.25',
            src: "./assets/images/kravMaga2.jpg",
            alt: "kravMaga2",
        },
        {
          text: 'טקס סיום קומ"כ 2.07',
          src: "./assets/images/endKumack1.jpg",
          alt: "endKumack1",
        },
        {
          text: 'טקס סיום קומ"כ 2.07',
          src: "./assets/images/endKumack2.jpg",
          alt: "endKumack2",
        },
        {
          text: 'טקס סיום קומ"כ 2.07',
          src: "./assets/images/endKumack4.jpg",
          alt: "endKumack4",
        },
        {
          text: 'טקס סיום קומ"כ 2.07',
          src: "./assets/images/endKumack5.jpg",
          alt: "endKumack5",
        },
        {
            text: 'טקס מצטיינים מפקדה - 6.05 ',
            src: "./assets/images/mifkadaMitztainim.JPG",
            alt: "mifkadaMitztainim",
        },
        {
            text: 'טקס מצטיינים מפקדה - 6.05 ',
            src: "./assets/images/mifkadaMitztainim1.JPG",
            alt: "mifkadaMitztainim1",
        },
        {
            text: 'סיום קורס משקי צפ"ה - 21.5',
            src: "./assets/images/tzapa1.jpg",
            alt: "tzapa1",
        },
        {
            text: 'סיום קורס משקי צפ"ה - 21.5',
            src: "./assets/images/tzapa2.jpg",
            alt: "tzapa2",
        },
        {
            text: 'סיום קורס משקי צפ"ה - 21.5',
            src: "./assets/images/tzapa3.jpg",
            alt: "tzapa3",
        },
        {
            text: 'סיום קורס משקי צפ"ה - 21.5',
            src: "./assets/images/tzapa4.jpg",
            alt: "tzapa4",
        },
        {
            text: 'סיום קורס משקי צפ"ה - 21.5',
            src: "./assets/images/tzapa5.jpg",
            alt: "tzapa5",
        },
        {
            text: 'טקס סיום השלמה חיילית - 23-24.07 ',
            src: "./assets/images/hashlama.jpg",
            alt: "hashlama",
        },
        {
            text: 'החלפת מפ מבצעים -  21-22.7.25',
            src: "./assets/images/mivtzaimMp.jpg",
            alt: "mivtzaimMp",
        },
        {
            text: 'החלפת מפ מבצעים -  21-22.7.25',
            src: "./assets/images/mivtzaimMp1.jpg",
            alt: "mivtzaimMp1",
        },
        {
            text: 'טקס הענקת  תגיות קורס חוקרים - 23.2.25',
            src: "./assets/images/investegators1.jpg",
            alt: "investegators1",
        },
        {
            text: 'טקס הענקת  תגיות קורס חוקרים - 23.2.25',
            src: "./assets/images/investegators2.jpg",
            alt: "investegators2",
        },
        {
          text: 'טקס סיום קומ"כ 23-27.07',
          src: "./assets/images/endKumack3.jpg",
          alt: "endKumack2",
        },
        {
          text: 'טקס סיום קומ"כ 23-27.07',
          src: "./assets/images/endKumack6.jpg",
          alt: "endKumack6",
        },
        {
          text: 'טקס סיום קורס רס"רים - 23.07',
          src: "./assets/images/rasarit.JPG",
          alt: "rasarit",
        },
        {
          text: 'טקס סיום קורס רס"רים - 23.07',
          src: "./assets/images/rasarit1.JPG",
          alt: "rasarit1",
        },
        {
          text: 'טקס סיום קורס רס"רים - 23.07',
          src: "./assets/images/rasarit2.JPG",
          alt: "rasarit2",
        },
        {
          text: 'טקס סיום קורס רס"רים - 23.07',
          src: "./assets/images/rasarit3.JPG",
          alt: "rasarit3",
        },
        {
          text: 'מדור מבצעים נכנסים לענף לוגיסטיקה - 10.02',
          src: "./assets/images/mivtzaimLog.jpg",
          alt: "mivtzaimLog",
        },
        {
          text: 'מדור מבצעים נכנסים לענף לוגיסטיקה - 10.02',
          src: "./assets/images/mivtzaimLog1.jpg",
          alt: "mivtzaimLog",
        },
        {
          text: 'מדור מבצעים נכנסים לענף לוגיסטיקה - 10.02',
          src: "./assets/images/mivtzaimLog2.jpg",
          alt: "mivtzaimLog",
        },
        {
          text: 'מסדר הנפה כלל בה"די - 21.07',
          src: "./assets/images/hanafa1.JPG",
          alt: "hanafa1",
        },
        {
          text: 'מסדר הנפה כלל בה"די - 21.07',
          src: "./assets/images/hanafa2.jpg",
          alt: "hanafa2",
        },
        {
          text: 'ערב מ"פ - 25.02 ',
          src: "./assets/images/mpEve.png",
          alt: "mpEve",
        },
        {
          text: 'ערב מ"פ - 25.02 ',
          src: "./assets/images/mpEve1.png",
          alt: "mpEve",
        },
        {
          text: 'פרידה מקטנא"ר- 24.07',
          src: "./assets/images/kantar.JPG",
          alt: "kantar",
        },
        {
          text: 'פרידה מקטנא"ר- 24.07',
          src: "./assets/images/kantar1.JPG",
          alt: "kantar",
        },
        {
          text: 'פרידה מראש מערך חינוך - 04.07 ',
          src: "./assets/images/hinuchMaarach.jpg",
          alt: "hinuchMaarach",
        },
        {
          text: 'פרידה מראש מערך חינוך - 04.07 ',
          src: "./assets/images/hinuchMaarach1.png",
          alt: "hinuchMaarach",
        },
        {
          text: ' אימון קרב מגע גולני וצנחנים - 12.02',
          src: "./assets/images/golaniKravMaga.jpg",
          alt: "golaniKravMaga",
        },
        {
          text: ' סיור בכירים במרכז מורשת - 16.2.25',
          src: "./assets/images/moreshet.jpg",
          alt: "",
        },
        {
          text: ' סיור בכירים במרכז מורשת - 16.2.25',
          src: "./assets/images/moreshet1.jpg",
          alt: "",
        },
        {
          text: ' סיור בכירים במרכז מורשת - 16.2.25',
          src: "./assets/images/moreshet2.jpg",
          alt: "",
        },
        {
          text: 'יום פרט - 8-10.07',
          src: "./assets/images/prat1.png",
          alt: "prat1",
        },
        {
          text: 'יום פרט - 8-10.07',
          src: "./assets/images/prat2.jpg",
          alt: "prat2",
        },
        {
          text: 'יום פרט - 8-10.07',
          src: "./assets/images/prat3.png",
          alt: "prat2",
        },
        {
          text: 'טקס סיום השלמות אחוד - 9-10.7.25',
          src: "./assets/images/hashlamaAshud1.JPG",
          alt: "hashlamaAshud1",
        },
        {
          text: 'טקס סיום השלמות אחוד - 9-10.7.25',
          src: "./assets/images/hashlamaAshud2.JPG",
          alt: "hashlamaAshud2",
        },
        {
          text: 'טקס סיום השלמות אחוד - 9-10.7.25',
          src: "./assets/images/hashlamaAshud3.JPG",
          alt: "hashlamaAshud2",
        },
        {
          text: 'תרגיל כיבוי אש - 03.02',
          src: "./assets/images/firePractice.JPG",
          alt: "firePractice",
        },
        {
          text: 'תרגיל כיבוי אש - 03.02',
          src: "./assets/images/firePractice1.JPG",
          alt: "firePractice",
        },
        {
          text: 'טקס פרידה מראש אט"ל - 17.08',
          src: "./assets/images/roshAtal.png",
          alt: "roshAtal",
        },
        {
          text: 'טקס פרידה מראש אט"ל - 17.08',
          src: "./assets/images/roshAtal1.png",
          alt: "roshAtal",
        },
        {
          text: 'טקס פרידה מראש אט"ל - 17.08',
          src: "./assets/images/roshAtal2.png",
          alt: "roshAtal",
        },
        {
          text: 'מסע תגיות קורס מפקדים  - 13.08',
          src: "./assets/images/masa1.png",
          alt: "masa1",
        },
        {
          text: 'מסע תגיות קורס מפקדים  - 13.08',
          src: "./assets/images/masa2.png",
          alt: "masa2",
        },
        {
          text: 'מסע תגיות קורס מפקדים  - 13.08',
          src: "./assets/images/masa3.png",
          alt: "masa3",
        }
      ],
    };
  },
  methods: {},
};
</script>

<style scoped>
#images {
  display: flex;
  justify-content: center;
  align-content: center;
  flex-wrap: wrap;
}

.image-card {
    margin: 0rem 0.3rem;
    text-align: center;
    align-content: center;
}

.image-png {
  max-height: 30rem;
  max-width: 25rem;
}

.img-text {
    color: #EDFAFF;
    font-family: "carmela";
}
</style>
