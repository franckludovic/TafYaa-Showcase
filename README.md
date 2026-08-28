<div align="center">

# Tafyaa - African Family Tree Platform

**Build your African family tree. Preserve your heritage. Connect across generations.**

</div>

---

## What is Tafyaa?

**Tafyaa** is a culturally-aware, collaborative family tree platform built specifically with **African family structures and storytelling traditions** in mind. The name *Tafyaa* - derived from African heritage - embodies the spirit of gathering, remembrance, and lineage.

Unlike generic genealogy platforms, Tafyaa was built from the ground up to answer a simple but profound question:

> *"How do you represent the full richness of an African family - polygamous unions, oral traditions, cross-continental diaspora - in a single digital space?"*

This project is the answer.

---

## Core Philosophy

Most genealogy tools were designed for a single cultural context. They assume monogamous family units, written records, and nuclear family structures. Tafyaa takes a different approach:

- **Oral history is primary.** Audio recordings of elders are a first-class feature, not an afterthought.
- **Complex family structures are embraced.** Polygamous marriages are fully supported and accurately visualised.
- **Collaboration is at the heart.** A tree is not one person's property - it belongs to the whole family.
- **Connection across borders.** The African diaspora is global. Tafyaa helps reconnect families scattered across continents.

---

## Key Features

### 🎙️ Oral History Preservation
Capture the voices and stories of your elders before they are lost. Each family member's profile supports audio recordings, allowing spoken narratives - stories, names, proverbs, and history - to live alongside their biographical information. Recordings are played back with a built-in waveform audio player powered by WaveSurfer.js.

### 🌳 Interactive Family Tree Visualisation
The tree is rendered as a beautiful, interactive graph using **ReactFlow** and **react-d3-tree**, supporting:
- Horizontal and vertical tree layouts
- Zoom, pan, and navigation controls
- Custom node rendering per person (photo, name, dates)
- Export to PDF and image formats

### 👨‍👩‍👧‍👦 Polygamous Family Structure Support
Tafyaa uniquely models **polygamous marriages** as distinct relationship entities, allowing one person to have multiple spouses while their children are correctly linked to both parents. The SVG relationship model distinguishes:
- Standard (monogamous) union
- Marriage union (with cultural designations)
- Multi-spouse unions rendered with dedicated link types

### 🤝 Collaborative Tree Editing
Family trees are shared spaces. Multiple people can collaborate on the same tree with a granular, **role-based permission system**. Collaboration features include:
- Email and QR-code invitations
- Join requests (public trees can be requested to join)
- Activity logs tracking who changed what and when

### 🔍 Cross-Tree Suggestions and Relative Discovery
Tafyaa's suggestion engine compares people across different trees and surfaces potential relative matches - people who may appear in two separate trees but are actually the same individual. This enables families to **discover unknown connections** and optionally merge their trees.

### 🌐 Global Family Search
A public tree search allows anyone to search for families by name, clan, or location. This makes Tafyaa a living directory of African lineages, enabling members of the diaspora to find branches of their family they never knew were on the platform.

### 📖 Stories and Events Timeline
Beyond biographical data, each person's profile supports:
- **Stories** - written narratives, memories, and history entries
- **Events** - dated milestones (births, marriages, migrations, achievements)
- **Media** - photos and documents stored via Cloudinary

All of these form a rich timeline for every individual in the tree.

### 📤 Export and Sharing
Trees and individual profiles can be exported as:
- **PDF documents** (via jsPDF and html2pdf.js)
- **PNG/JPEG images** (via html-to-image and html2canvas)
- **QR codes** for sharing a public tree link

---

## 🛡️ Roles and Permissions

Tafyaa uses a **four-tier role system** to manage what each collaborator can do within a tree:

| Role | Description |
|------|-------------|
| 👑 **Admin** | Full control. Can manage all members, delete the tree, and perform any action. |
| 🛡️ **Moderator** | Can add, edit, and delete persons and content. Can manage members and invites. Cannot delete the tree. |
| ✏️ **Editor** | Can add and edit persons and content within their own **lineage branch**. Cannot delete or manage members. |
| 👁️ **Viewer** | Read-only access. Can browse the tree and export it, but cannot make any changes. |

Permissions are enforced both client-side (UI gating) and server-side (Netlify Functions + Firestore security rules). Editors are additionally restricted to their own **lineage** - the branch of the tree they belong to - preventing unauthorised edits outside their family line.

---

**Live Demo:** (Taf'Yaa)[https://tafyaa.netlify.app/]

<div align=center>

<img width="1358" height="6476" alt="image" src="https://github.com/user-attachments/assets/e7c1ac41-d7e5-4966-a131-888b8521b815" />

</div>

---

**Built with ❤️ to honour African heritage.**
