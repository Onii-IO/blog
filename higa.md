---
title: Onii - Version 1.0
category: Update
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit. At atque debitis delectus, dignissimos dolores eligendi eos ex, harum magnam numquam omnis quidem reprehenderit sunt? Ad impedit laboriosam quos recusandae vel.
---

# Higa

## What is Higa ?
It's a random Discord API package builded with randomness by fantomitechno.

## Why a new one as Discord.js exist and is powerfull ?
Just because I want to train myself and doing a project like that can be very interesting. More over, I don't agree with some of the ways Discord.js do some things so as I can't have myself to understand its code to do a fork, I decided to write my own library to do things like I want.

## Finaly, why the name Higa ?
Higa is a character from Swort Art Online (really good anime 🙃) and I wanted a reference to that anime so I thought about the personnages I liked the most : Kayaba, Yui, Eugeo... And after some thinking, I remembered this personnage : a developper for the Fluctlight project, exactly who I wanted ! ^^

![Higa](https://repository-images.githubusercontent.com/449401958/bc8d5876-fec3-4e0c-a047-be19a89068ca)

~~~javascript
// @ts-ignore
const fetcher = (...args: any[]) => fetch(...args).then((res) => res.json());
// @ts-ignore
const fetcherText = (...args: any[]) => fetch(...args).then((res) => res.text());

const fetcherParams = (url: string, path: string) => {
    const myHeaders = new Headers();
    myHeaders.append('Content-Type', 'application/x-www-form-urlencoded');

    const urlencoded = new URLSearchParams();
    urlencoded.append('path', path);

    return fetch(url, {
        method: 'POST',
        headers: myHeaders,
        body: urlencoded,
        redirect: 'follow'
    })
        .then((response) => response.json())
        .catch((error) => console.log('error', error));
};

const fetcherQuery = (url: string, query: string, method?: string) => {
    console.log();
};

export default fetcher;
export { fetcherParams, fetcherQuery, fetcherText };

~~~

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3


> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.

Three or more...

---

Hyphens

***

Asterisks

___

Underscores
