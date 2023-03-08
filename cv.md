# rsschool-cv

## Nikolay Krishtopa

### Frontend developer

- Location: Batumi
- Ready to relocate
- Ready for business trips

### Contact information:

- phone: +995-579-05-44-95
- Telegram: @Nikolay_Krishtopa
- [Email](mailto:nikolay.krishtopa@gmail.com)
- [LinkedIn](https://www.linkedin.com/in/nikolay-krishtopa/)

### Technologies stack:

- HTML
- CSS (BEM, SASS, SCSS)
- JavaScript
- Typescript
- ReactJS
- VueJS
- Redux, RTK, Redux thunk
- TailwindCSS
- Webpack
- NodeJS

### Education:

#### Bauman Moscow Technical State University, master degree

- 2004 - 2010
- Faculty: Special machinery
- Speciality: Spacecrafts and boosters design
- Grade: 4.5

#### Yandex Practicum (additional education)

- 2022 - 2023
- Speciality: Web development

#### RS school (additional education)

- 2023 - present
- Speciality: JavaScript/Front-end

### Work experience:

#### Weber, frontend developer

- 2022 - present
- working as a part of the team of frontend developers for the project of web application for photographers portfolio. Technical stack used: Typescript, React, Redux toolkit, SCSS, HTML

#### Hash INC, frontend developer

- 2022 -2023
- Development of the online game integrated into the Telegram chatbot. The team was counting up to 6 developers, work process per agile/scrum. Tech stack: JS, Three.JS, Webpack, HTML, CSS.

#### The Boeing Company, design engineer/manufacturing engineer

- 2011 -2022
- focusing on the sustain of the airplanes production. Lean/scrum methods. The team was counting up to 25 persons. Daily work in English language. Long-term business trips to the head office and factory in USA. Have an experience of the leading the group up to 15 persons. Have improved a few work process. Many times got an excellent feedback from the management and customers. Employee of the year in 2021.

### Languages:

- Russian - native
- English - upper-intermediate

### About myself

I extremely love being involved in the creating of some fantastic products, mostly that’s why I had been an engineer for the Boeing company for a long time: when you’re looking at the taking off airplane which was designed and produced with your even small contribution – that’s absolutely breathtaking.

However, after some years I realized that was time to move further because it had been gradually harder to find personal challenges and being continuously improving my skills. It was time to try to leave “comfort zone” and open something new for me. I got interested at the web development (as a hobby first) and after some practice I decided to move to this business. As I am pretty experienced with work for huge international company, I have English fluent language skills (Upper-intermediate), aware of Lean and SCRUM. In addition, my experience allowed me to improve my soft-skills. I’m always open for studying something new and never avoid that. I’m never scared of the difficult tasks but get motivated of them.

I was leading the team counting from 10 to 12 people working for the big and very important project. After implementing that I got very high assessment from my management.

When I have some time for myself I like skiing and cycling as well as reading. Also I like travelling.

### The code example

```
export const createNewSection = createAsyncThunk<
  void,
  { newSectionName: string; token: string },
  { rejectValue: string }
>(
  'sections/createSection',
  async function ({ newSectionName, token }, { dispatch, rejectWithValue }) {
    try {
      const res = await fetch(`${BASE_URL}sections?section=${newSectionName}`, {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({ token }),
      })
      if (!res.ok) {
        throw new Error('Ошибка при создании новой секции на сервере')
      } else dispatch(getSections())
    } catch (err: any) {
      return rejectWithValue(err.message)
    }
  }
)
```
