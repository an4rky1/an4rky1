# 💻 Roman Ivanov | Fullstack Developer

> _"Code is poetry, architecture is logic."_

<div align="center">
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</div>

---

## 📜 `RESUME.TS`

<table>
<tr>
<td width="50%">

```typescript
/**
 * @summary
 * Fullstack Developer specializing in
 * Next.js, Laravel, and Microservices.
 * Building scalable web applications,
 * developer tools, and SaaS platforms.
 * @author Roman Ivanov
 * @location Ukraine
 */

// ─── Types & Interfaces ──────────────

type ExperiencePeriod = `${number} - ${number | 'Present'}`;
type LanguageLevel = 'Native' | 'Fluent' | 'Conversational';

interface Developer {
  readonly role: string;
  readonly location: string;
  readonly email: string;
  readonly languages: Record<string, LanguageLevel>;
  readonly stack: TechStack;
  readonly experience: Experience[];
  readonly education: Education[];
  readonly projects: Project[];
}

enum Framework {
  NextJS = 'Next.js',
  React = 'React',
  Laravel = 'Laravel',
  Symfony = 'Symfony',
  VueJS = 'Vue.js',
  NestJS = 'NestJS',
}

enum Language {
  TypeScript = 'TypeScript',
  JavaScript = 'JavaScript',
  PHP = 'PHP',
  Python = 'Python',
  SQL = 'SQL',
}

enum Database {
  PostgreSQL = 'PostgreSQL',
  Redis = 'Redis',
  Supabase = 'Supabase',
  DrizzleORM = 'Drizzle ORM',
}

enum Tool {
  Docker = 'Docker',
  AWS = 'AWS',
  GCP = 'GCP',
  GraphQL = 'GraphQL',
  gRPC = 'gRPC',
  Git = 'Git',
  Linux = 'Linux',
}

interface TechStack {
  frameworks: Framework[];
  languages: Language[];
  databases: Database[];
  tools: Tool[];
}
```

</td>
<td width="50%">

```typescript
interface Experience {
  readonly title: string;
  readonly company: string;
  readonly period: ExperiencePeriod;
  readonly stack: string[];
  readonly achievements: string[];
}

interface Education {
  readonly degree: string;
  readonly institution: string;
  readonly period: ExperiencePeriod;
}

interface Project {
  readonly name: string;
  readonly description: string;
  readonly stack: string[];
  readonly status: 'completed' | 'in-progress';
  readonly codeLink?: string;
  readonly demoLink?: string;
}

// ─── Implementation ──────────────────

const romanIvanov: Developer = {
  role: 'Next.js Developer & Fullstack Engineer',
  location: 'Ukraine',
  email: 'roman.ivanov@email.com',
  languages: {
    Ukrainian: 'Native',
    English: 'Fluent',
    Russian: 'Fluent',
  },
  stack: {
    frameworks: [
      Framework.NextJS, Framework.React,
      Framework.Laravel, Framework.Symfony,
      Framework.VueJS, Framework.NestJS,
    ],
    languages: [
      Language.TypeScript, Language.JavaScript,
      Language.PHP, Language.Python, Language.SQL,
    ],
    databases: [
      Database.PostgreSQL, Database.Redis,
      Database.Supabase, Database.DrizzleORM,
    ],
    tools: [
      Tool.Docker, Tool.AWS, Tool.GCP,
      Tool.GraphQL, Tool.gRPC, Tool.Git,
      Tool.Linux,
    ],
  },
  experience: [
    {
      title: 'Next.js Developer',
      company: 'Nimbus Systems',
      period: '2024 - 2025',
      stack: ['React', 'Next.js', 'TypeScript', 'SSR/SSG'],
      achievements: [
        'Built production React/Next.js apps',
        'Implemented SSR and static generation',
        'Optimized bundle size & Core Web Vitals',
      ],
    },
    {
      title: 'Laravel Fullstack Developer',
      company: 'CipherTech',
      period: '2024 - 2025',
      stack: ['Laravel', 'Vue.js', 'REST APIs', 'Auth'],
      achievements: [
        'Developed RESTful APIs & real-time features',
        'Integrated Vue.js frontend with Laravel',
        'Implemented auth and payment systems',
      ],
    },
    {
      title: 'Symfony Fullstack Developer',
      company: 'Vertex Labs',
      period: '2023 - 2024',
      stack: ['Symfony', 'PostgreSQL', 'Redis', 'Elasticsearch'],
      achievements: [
        'Built enterprise apps with Symfony',
        'Worked with PostgreSQL, Redis, Elasticsearch',
        'Implemented REST APIs & microservices',
      ],
    },
    {
      title: 'Frontend Developer',
      company: 'Freelance',
      period: '2022 - 2023',
      stack: ['HTML', 'CSS', 'JavaScript', 'React.js'],
      achievements: [
        'Created responsive websites',
        'Worked with React.js & state management',
        'Collaborated on UI/UX implementation',
      ],
    },
  ],
  education: [
    {
      degree: 'Computer Science',
      institution: 'Donbas State Engineering Academy',
      period: '2018 - 2023',
    },
    {
      degree: 'Applied Mathematics',
      institution: 'Horlivka Technical College',
      period: '2011 - 2014',
    },
  ],
  projects: [
    {
      name: 'ASCII Terminal',
      description: 'Matrix-style ASCII art generator',
      stack: ['Next.js 16', 'TypeScript', 'Supabase'],
      status: 'completed',
      codeLink: 'https://github.com/anarky/ascii',
    },
    {
      name: 'News Platform',
      description: 'Real-time news aggregation',
      stack: ['Next.js 16', 'React Query', 'Framer Motion'],
      status: 'completed',
      codeLink: 'https://github.com/anarky/news',
    },
    {
      name: 'Pixel Art Converter',
      description: 'Image processing pipeline',
      stack: ['Next.js 14', 'PostgreSQL', 'Drizzle ORM', 'Sharp'],
      status: 'completed',
      codeLink: 'https://github.com/anarky/pixel-art-converter',
    },
    {
      name: 'Blog Platform',
      description: 'FSD blog with full-text search',
      stack: ['Next.js 14', 'PostgreSQL', 'Drizzle ORM', 'Zod'],
      status: 'completed',
      codeLink: 'https://github.com/anarky/blog-platform',
    },
    {
      name: 'SaaS Platform',
      description: 'Microservices with GraphQL & gRPC',
      stack: ['NestJS 11', 'GraphQL', 'gRPC', 'CQRS'],
      status: 'in-progress',
    },
    {
      name: 'Core Framework',
      description: 'Nx monorepo for NestJS microservices',
      stack: ['NestJS 11', 'Nx', 'TypeScript', 'Express 5'],
      status: 'in-progress',
    },
  ],
};

// ─── Exports ─────────────────────────

export type { Developer, Experience, Education, Project, TechStack };
export { Framework, Language, Database, Tool };
export default romanIvanov;
```

</td>
</tr>
</table>

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=romanivanov&show_icons=true&theme=transparent&hide_border=true" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=romanivanov&layout=compact&theme=transparent&hide_border=true" alt="Top Languages" />
</div>

---

## 📬 Connect With Me

<p align="center">
  <a href="mailto:roman.ivanov@email.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://github.com/romanivanov"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://linkedin.com/in/romanivanov"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://t.me/romanivanov"><img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" /></a>
</p>

---

> _"The best code is the code that never needs to be written. The second best is the code that works exactly as intended."_

<div align="center">
  <sub>Built with ❤️ using Next.js, TypeScript & TailwindCSS</sub>
</div>
