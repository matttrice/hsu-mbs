---
background-image: './images/scroll.jpg'
routeAlias: intro
info: |
  ## MBS Lesson 1
title: Introduction to Reasoning
layout: intro
---

“When one learns to read, one learns a peculiar way of behaving of which physical immobility is only one feature. Self restraint is a challenge not only to the body but to the mind as well. Sentences paragraphs and pages unfold slowly, in sequence and according to a logic that is far from intuitive...  the literate person must learn to be reflective and analytical, patient and assertive always poised, after due consideration to say no to a text."

Neil Postman – The Disappearance of Childhood

---
title: Bible Layout
background: bg-slate-500
routeAlias: bible-layout
layout: default
---

<div text-2xl class="-mt-8">Old Testament: 39 books</div>

<div class='grid grid-cols-[auto_auto_auto_auto_auto]' text-left>
  <div v-click='1'>
   <div underline> Law <sup>(5)</sup> </div>
   <div text-sm> 
   <div> Genesis </div>
   <div> Exodus </div>
   <div> Leviticus </div>
   <div> Numbers </div>
   <div> Deuteronomy </div> 
   </div>
  </div>
  <div v-click='2'>
  <div underline> History <sup>(12)</sup> </div>
  <div text-sm> 
    <div> Joshua </div>
    <div> Judges </div>
    <div> Ruth </div>
    <div> 1 & 2 Samuel </div>
    <div> 1 & 2 Kings </div>
    <div> 1 & 2 Chronicles </div>
    <div> Ezra </div>
    <div> Nehemiah </div>
    <div> Esther </div>
    </div>
  </div>
  <div v-click='3'>
   <div underline> Poetry <sup>(5)</sup> </div>
   <div text-sm> 
    <div> Job </div>
    <div> Psalms </div>
    <div> Proverbs </div>
    <div> Ecclesiastes </div>
    <div> Song of Solomon </div>
  </div>
  </div>
  <div v-click='4'>
    <div underline> MajorProphets <sup>(5)</sup> </div>
    <div text-sm> 
    <div> Isaiah </div>
    <div> Jeremiah </div>
    <div> Lamentations </div>
    <div> Ezekiel </div>
    <div> Daniel </div>
    </div>
  </div>
  <div v-click='5'>
    <div underline> MinorProphets <sup>(12)</sup> </div>
    <div text-sm> 
    <div> Hosea </div>
    <div> Joel </div>
    <div> Amos </div>
    <div> Obadiah </div>
    <div> Jonah </div>
    <div> Micah </div>
    <div> Nahum </div>
    <div> Habakkuk </div>
    <div> Zephaniah </div>
    <div> Haggai </div>
    <div> Zechariah </div>
    <div> Malachi </div>
  </div>
  </div>
</div>

 ----

<div v-click='6' text-2xl>New Testament: 23 books</div>

<div class='grid grid-cols-[auto_auto_auto_auto_auto]' text-left>
    <div v-click='7'>
      <div underline>Gospel <sup>(4)</sup></div>
        <div text-sm> 
            <div>Matthew</div>
            <div>Mark</div>
            <div>Luke</div>
            <div>John</div>
        </div>
      </div>
  <div v-click='8'>
    <div underline>ChurchHistory <sup>(1)</sup></div>
        <div text-sm> 
        <div>Acts</div>
    </div>
  </div>
  <div v-click='9'>
  <div underline>Prophecy <sup>(1)</sup></div>
        <div text-sm> 
            <div>Revelation</div>
        </div>
  </div>
  <div v-click='10'>
  <div underline>Letters to Churches <sup>(9)</sup></div>
    <div text-sm>
      <div>Romans</div>
      <div>1 & 2 Corinthians</div>
      <div>Galatians</div>
      <div>Ephesians</div>
      <div>Philippians</div>
      <div>Colossians</div>
      <div>1 & 2 Thessalonians</div>
  </div>
  </div>
    <div v-click='11'>
    <div underline>Letters to Individuals <sup>(12)</sup></div>
      <div text-sm>
       <div>1 & 2 Timothy</div>
       <div>Titus</div>
       <div>Philemon</div>
       <div>Hebrews</div>
       <div>James</div>
       <div>1 & 2 Peter</div>
       <div>1, 2 & 3 John</div>
       <div>Jude</div>
      </div>
      </div>
  </div>
  <div v-click='12'>How does theAuthor think?</div>

---
title: Methods of Reason
routeAlias: bible-reasoning
layout: full
---
  
# Methods of Reason
  
<div class="grid grid-cols-[1fr_1fr]">
<div class="txt-carnal txt-4xl mx-auto">What method of reason is sbest if you don't know the complete picture?</div>

<div class="txt-spirit txt-4xl mx-auto">How do you start a puzzle?</div>
    <div v-click="1" class="txt-carnal bg-carnal mbs-col-head txt-4xl mx-auto"> Inductive</div>
    <div v-click="2" class="txt-spirit bg-spirit mbs-col-head txt-4xl">Deductive</div> 
    <div class="grid grid-cols-[1fr_1fr]">
        <div v-click="3" class="txt-carnal bg-carnal text-2xl" height="100px"> 
            <div class="txt-3xl">Small</div>
            <div>Specific</div>
            <svg height="55px">
                <circle cx="150" cy="30" r="10" stroke="black" stroke-width="3" fill="black" />
            </svg>
      </div>
        <div v-click="4" class="txt-carnal bg-carnal text-2xl">
            <div>Big</div>
            <div>General</div>
            <svg width="500" height="500">
                <circle cx="400" cy="40" r="80" stroke="black" stroke-width="3" fill="black" />
                <line x1="20" y1="30" x2="400" y2="30" stroke="black" stroke-width="25" />
            </svg>
        </div>
    </div>
    <div class="grid grid-cols-[1fr_1fr]">
        <div v-click="5" class="txt-spirit bg-spirit text-2xl">
            <div>Big</div>
            <div>General</div>
        <div v-click="6">
            <div class="txt-spirit">
                <div>Small</div>
                <div>Specific</div>
            </div>
        </div>
        </div>
    </div>
</div>

