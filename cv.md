# RS School Student CV

## Personal Information

![My friendly-aggressive selfie here](https://i.ibb.co/S550HNx/20201220-171407.jpg)

**Name**: Dmitriy Vnuchkov  
**Age**: 30  
**Origin**: Tashkent, Uzbekistan  
**Email**: dmitriy.vnuchkov@gmail.com
**Discord**: Dmitriy V (@DeevDevs)

**Bio**: I am a teacher of English language, who has decided to make an attempt in shifting from language teaching to information technology. 18 months have passed since my first deep dive into programming, and I feel more than excited about the doors to open, knowledge to gain, and practices to do. So far, I have participated in a number of projects during my studies. I was mainly learning online all by myself, using YouTube and Udemy courses.

Since I love working with computers, programming is fun to me. Obviously, I feel tired after sitting and coding for several hours. It is a nice exercise for my brain because coding implies thinking logically and analytically. Sometimes I spend too much time making things perfect, so I try to stay away from this obsessive idea to complete tasks to the nail at once. On the other hand, it never takes much time to pull my socks up. They say "Coding is fun!", and I agree with that.

## Qualifications

### _Unrelated to IT_

**2012 - Bachelor in English Philology** (_Uzbek State University of World Languages_, _Tashkent_)  
**2019 - Master of Art in Teaching English to Speakers of Other Languages** (_University of Nicosia_, _Cyprus_)

### _Related to IT_

**2021 - The Complete Javascript Course: From Zero to Expert** (_Udemy Platform_)  
**2022 - CSS - The Complete Guide** (_Udemy Platform_)  
**2022 - Node.js, Express, MongoDB and More: The Complete Bootcamp** (_Udemy Platform_)

### _Languages_

**Russian** - Native  
**English** - Advanced

## Skills

**HTML & CSS** - Intermediate  
**Javascript** - Intermediate  
**Node.js** - Advanced Beginner  
**Express** - Advanced Beginner

### _Code Example_

```javascript
  async displayFrontProjectDetails(projectId) {
    try {
      let projectData;
      const idNum = parseInt(projectId);
      if (this.projectDetails[idNum - 1].length === 0) {
        const res = await axios({
          method: 'GET',
          url: `/details?prnumber=${idNum}`,
        });
        if (res.data.message === 'success') {
          projectData = [res.data.detailsData.detailsLeft, res.data.detailsData.detailsRight];
          this.projectDetails[idNum - 1] = projectData;
        }
      } else projectData = this.projectDetails[idNum - 1];
      this.wheelDetails.forEach((element, i) => {
        element.firstChild.textContent = projectData[i];
        element.style.opacity = 1;
      });
    } catch (err) {
      this.wheelDetails.forEach((element, i) => {
        element.firstChild.textContent =
          'Oops... Something went wrong. Information about this project is not accessible at the moment. Please, try again later.';
        element.style.opacity = 1;
      });
    }
  }
```

## Experience

I have not worked in IT so far. Yet, I have participated in a number of projects during my studies, and I have two pet-projects, too.

## Projects

**Mapty** - an application for creating workout records. [See the code and description in Git](https://github.com/DeevDevs/dd-mapty-app) and [have a look at the deployed project](https://deevdevs-mapty-app.netlify.app/).

**Bankist: Homepage** - presentation of practical skills in HTML & CSS. [See the code and description in Git](https://github.com/DeevDevs/dd-bankist-homepage) and [have a look at the deployed project](https://deevdevs-bankist-homepage.netlify.app/).

**Bankist: Application** - presentation of practical skills in working with Arrays in Javascript. [See the code and description in Git](https://github.com/DeevDevs/dd-bankist-app) and [have a look at the deployed project](https://deevdevs-bankist-app.netlify.app/).

**Natours** - an application for booking tours. [See the code and description in Git](https://github.com/DeevDevs/dd-natours) and [have a look at the deployed project](https://deevdevs-natours.herokuapp.com/).

**Forkify** - an application for searching for and adding recipes. [See the code and description in Git](https://github.com/DeevDevs/dd-forkify-app) and [have a look at the deployed project](https://deevdevs-forkify-app.netlify.app/).

**Connect Four** - my pet project. It is a browser game based on a popular tabletop game. [See the code and description in Git](https://github.com/DeevDevs/dd-connect-four) and [have a look at the deployed project](https://deevdevs-connect-four.netlify.app/).

**Pig Game** - a simple game with numbers - my first project experience. [See the code and description in Git](https://github.com/DeevDevs/dd-pig-game) and [have a look at the deployed project](https://deevdevs-pig-game.netlify.app/).

**My First Portfolio** - my pet project. This is my first attempt to create a web portfolio. [See the code and description in Git](https://github.com/DeevDevs/dd-my-portfolio) and [have a look at the deployed project](https://deevdevs-my-portfolio.herokuapp.com/).
