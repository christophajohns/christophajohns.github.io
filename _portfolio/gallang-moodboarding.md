---
title: "Gallang - High Quality Moodboarding Assets"
excerpt: "<img src='/images/gallang/thumbnail.png' alt='Gallang - High Quality Moodboarding Assets' style='margin-bottom: 0.5rem; border: 1px solid lightgrey; max-height: 500px'><br/>Web app for collecting high-quality assets for moodboarding."
collection: portfolio
---

<figure>
  <img
    src="/images/gallang/thumbnail.png"
    alt="Gallang - High Quality Moodboarding Assets"
    style="border: 1px solid lightgrey"
  />
  <figcaption>
    Gallang is a web app for collecting high-quality assets for moodboarding.
  </figcaption>
</figure>

This project is part of the KTH Royal Institute of Technology course "DH2642: Interaction Programming and the Dynamic Web".

It was created by Christoph A. Johns, Yuqi Liu, Annetta Sillard, and Xiaoying Sun.

The application is publicly available on Heroku at <https://gallang.herokuapp.com>.

## Quick Overview

### Motivation

Designers often create mood-boards, for example using Pinterest or Miro, to explore the design space.
The images provided by these resources are often inconsistent in quality and the recommendation engines hinder, to some degree, truly imaginative and free inspiration.
A digital mood-board bringing together several different sources of high-quality media, for example, stock photography, art galleries, fonts, etc. could lead to more effective exploration of the design space.

### Results

In its current iteration, Gallang offers users the option to browse through and search for images from a reputable source, the [Cooper Hewitt (Smithsonian Art Museum)](https://collection.cooperhewitt.org/api/).
The user can like and save those images into collections (called "Galleries").
Based on the individual usage behavior (i.e. the user's likes), Gallang computes and displays recommendations for similar artists, institutions, media or types that the user might also be interested in.
When users want to continue their work in other design tools like Figma, they can download the images to their local machine for further use.
This way, Gallang offers users a way to be inspired and to collect high-quality mood boarding assets for their design projects.

## Features

We have implemented the following features:

- User authentication using Firebase (sign up, login, forgot password, edit user profile, delete user)
- Persisted application state using Firebase
- Home/browse page to view "featured" collections (i.e. images of objects from certain periods using the [Cooper Hewitt API](https://collection.cooperhewitt.org/api/)) and recommended images (only displayed if a user has liked at least three images)
- Search functionality using the [Cooper Hewitt API](https://collection.cooperhewitt.org/api/)
- Options to create, view and delete galleries (collections of images)
- Basic recommendation engine to return suggested images with similar medium, type, or participants from the [Cooper Hewitt API](https://collection.cooperhewitt.org/api/) based on a user's liked images
- Liked content page to view and download your liked images
- Profile page to view and edits one's user data and profile
- Drag-and-Drop images to add them to a gallery
