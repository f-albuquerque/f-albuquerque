```typescript
interface Workplace {
  company: string;
  position: string;
}

interface User {
  name: string;
  age: number;
  country: string;
  workplace: Workplace;
}

class About {
  public getData(): User {
    return {
      name: 'Fabio Silva',
      age: 24,
      country: 'Portugal',
      workplace: this.getCurrentWorkplace(),
    };
  }

  public getCurrentWorkplace(): Workplace {
    return {
      company: 'Zapp-Studio',
      position: 'Full Stack Developer',
    };
  }

  public getSkills(): string[] {
    return [
      'TypeScript',
      'Vue.js',
      'Nuxt.js',
      'Vuetify',
      'Bootstrap',
      'Node.js',
      'NestJS',
      'Docker',
    ];
  }

  public getFutureGoal(): string {
    return 'Contribute to open source projects';
  }
}
```
