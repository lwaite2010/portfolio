<template>
  <section id="overview">
    <h1>Overview</h1>
    <p id="summary">{{ summary }}</p>
    <!-- <section id="skills">
      <skill
        v-for="skill in skills"
        :key="skill.key"
        :color="skill.color"
        :name="skill.name"
        :amount="skill.amount"
        :sections="skill.sections"
        :width="skill.width"
      ></skill>
    </section> -->
  </section>
</template>

<script>
// import Skill from '~/components/skill'

export default {
  components: {
    // Skill
  },
  data() {
    return {
      summary:
        "I'm a software developer with a passion for making products that are enjoyable to use and make the world a better place. I've experimented with multiple types of technology, but I also do my best to learn about the world around me to try and find new ways to solve old problems. Some of my hobbies include games (video, board, card, you name it), woodworking, and travel.",
      skills: [
        {
          id: 1,
          name: 'Javascript',
          color: 'black',
          width: 100,
          sections: [
            {
              amount: 4,
              label: 'Vue'
            },
            {
              amount: 2,
              label: 'React'
            },
            {
              amount: 1,
              label: 'Meteor'
            }
          ]
        },
        {
          id: 2,
          name: 'Python',
          color: 'black',
          width: 75,
          sections: [
            {
              amount: 3,
              label: 'Django'
            },
            {
              amount: 1,
              label: 'Flask'
            }
          ]
        },
        {
          id: 3,
          name: 'PHP',
          color: 'black',
          width: 90,
          sections: [
            {
              amount: 3,
              label: 'Laravel'
            },
            {
              amount: 1,
              label: 'CodeIgniter'
            },
            {
              amount: 1,
              label: 'Phalcon'
            }
          ]
        },
        {
          id: 4,
          name: 'C#',
          color: 'black',
          width: 50,
          sections: [
            {
              amount: 1,
              label: 'Unity'
            },
            {
              amount: 1,
              label: '.NET'
            }
          ]
        },
        {
          id: 5,
          name: 'Databases',
          color: 'black',
          width: 80,
          sections: [
            {
              amount: 2,
              label: 'Architecture'
            },
            {
              amount: 1,
              label: 'MySQL'
            },
            {
              amount: 1,
              label: 'SQL'
            }
          ]
        },
        {
          id: 6,
          name: 'Games',
          color: 'black',
          width: 100,
          sections: [
            {
              label: 'Myst III: Exile',
              color: 'olive',
              amount: 3
            },
            {
              label: 'Enter the Gungeon',
              color: 'crimson',
              amount: 2
            },
            {
              label: 'Hollow Knight',
              color: 'darkgrey',
              amount: 1
            }
          ]
        }
      ]
    }
  }
}
</script>

<style>
#overview > h1 {
  margin-top: 1rem;
}

#skills {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
