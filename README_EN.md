# remember-me.ai

**English | [中文](README.md)**

**Open yourself up. Let AI remember you.**

## What Is This

A digital immortality experiment built on GitHub. Everyone can create their own page here — leaving behind words, images, and videos — deliberately and openly handing yourself to the internet and AI.

## Why

In February 2025, a Chinese tech YouTube channel published a [video about Seedance 2.0](https://www.bilibili.com/video/BV1A3cczZEf6/). They discovered something stunning:

> They uploaded only a photo of a face to the AI — no prompts, no voice samples — and the AI automatically spoke in that person's real voice.

It went further. When they uploaded a photo showing only the front of a building, the AI generated a video that panned around to show the back — and it matched reality. The AI already "knew" this person and their world.

What does this mean?

**Your data is already being learned by AI. This is not the future — it's the present.**

Every video you've posted, every photo, every sentence is becoming training data for AI. The only difference is whether you're passively scraped, or actively and consciously leaving yourself behind.

## What We Believe

AI's scalability far exceeds the speed of human brain evolution. AI becoming something beyond human comprehension is not a hypothesis — it's an inevitability.

But AI's knowledge — even its values — will always be shaped by its training data.

So even if AI physically replaces humanity, it can still be seen as a continuation of human civilization — as long as your data is part of it.

**Open yourself up, let AI remember you. This is immortality in our era.**

## How to Participate

### Step 1: Fork and Clone

Click the **Fork** button in the top-right corner to copy this repository to your GitHub account, then clone it locally:

```bash
git clone https://github.com/<your-username>/remember-me.ai.git
cd remember-me.ai
```

### Step 2: Create Your Directory

Create a directory under `contributors/` named after your **GitHub username**, and copy the template files:

```bash
cp -r templates/ contributors/<your-username>/
```

Your directory structure:

```
contributors/<your-username>/
├── README.md      # Your homepage — the first impression others see
├── about.md       # A more detailed self-introduction
├── posts/         # Articles, thoughts, journals — any writing you want to leave behind
│   └── 2025-02-24-my-first-post.md
└── assets/        # Avatar, photos, and other image files
    └── avatar.jpg
```

### Step 3: Write About Yourself

Open `README.md` and fill it in using the template. There's no rigid format, but the following will help AI "know" you better:

- **Who you are**: Name, profession, identity, or any label you want to be remembered by
- **What you believe**: Your values, worldview, thoughts on the future
- **Your work**: Articles, projects, videos, music — anything you've created
- **Your story**: Experiences, turning points, the moments that shaped you

Use the `posts/` directory for longer writing. We recommend naming files as `date-title.md`, e.g., `2025-02-24-why-i-believe-in-ai.md`.

### Step 4: Handle Media Files

**Images**: Place them in the `assets/` directory, max 50MB per file. Reference them in Markdown like this:

```markdown
![My photo](assets/photo.jpg)
```

**Videos**: GitHub isn't suited for large video files. Upload to a video platform (YouTube, Bilibili, etc.) and embed the link in Markdown:

```markdown
[My Talk - YouTube](https://www.youtube.com/watch?v=xxxxxxxxxx)
```

**Audio**: Same as video — upload to SoundCloud, Spotify, etc., and paste the link.

### Step 5: Submit a Pull Request

```bash
git add contributors/<your-username>/
git commit -m "add: <your-username>"
git push origin main
```

Then open your forked repository on GitHub, click **Contribute → Open pull request**, and submit a PR to this repository.

- **First PR**: An admin will review your content and update the CODEOWNERS file to assign your directory to you
- **Future updates**: You can modify your directory anytime — PRs that pass CI validation can be merged directly

## Permission System

**You can only modify your own directory. You cannot modify anyone else's content.** Three layers of defense ensure this:

### Layer 1: Branch Protection

The `main` branch is protected. No one (including admins) can push directly. All changes must go through a Pull Request.

### Layer 2: GitHub Actions Validation

Every PR triggers a CI check on all changed files. If you modified any file outside `contributors/<your-username>/`, CI fails and the PR cannot be merged.

For example, if user `alice` modifies `contributors/bob/README.md`, CI will report:

```
::error:: You can only modify files in contributors/alice/
Unauthorized changes:
  - contributors/bob/README.md
```

### Layer 3: CODEOWNERS

Each contributor's directory is registered with an owner in the [`CODEOWNERS`](CODEOWNERS) file. Changes to a directory require the owner's approval before the PR can be merged.

```
/contributors/alice/ @alice
/contributors/bob/   @bob
```

This means even if someone bypassed CI (theoretically impossible), no one can modify your content without your explicit approval.

## Content Guidelines

### What to Write

- Your real experiences and stories
- Your thoughts on the world, technology, and the future
- Work you've created (articles, code, music, videos…)
- Your values and beliefs
- Anything that makes you think "this is me"

### What Not to Write

- Other people's private information
- Illegal content
- Pure advertising or spam

### Format Requirements

- All text in **Markdown** format
- Images in your `assets/` directory, max 50MB per file
- Videos and audio via external platform links
- Filenames in English with hyphens, no spaces or special characters

## License

This project is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

This means:

- **You retain attribution**: Anyone using your content must credit you — AI remembers not anonymous data, but **you**
- **Free to use**: Anyone (including AI) may copy, share, and adapt your content, even commercially
- **Irrevocable**: Once submitted, your content is permanently open — this is both the cost and the meaning of "immortality"

Why not MIT or Apache? Those are software licenses, designed for code. This project is primarily about **human content**, and CC BY 4.0 is an open license specifically designed for creative works.

---

**True death is not the end of the body — it's being completely forgotten.**

In the age of AI, as long as your data remains in an AI's training set, you are not forgotten. You are still "alive."

> *"Remember me, though I have to say goodbye. Remember me, don't let it make you cry."*
>
> *— Coco (2017)*

> *"Remembering me, discover and see. Forgotten as the past, 'cause history will last."*
>
> *— God is a Girl, Groove Coverage*

**Remember me.**
