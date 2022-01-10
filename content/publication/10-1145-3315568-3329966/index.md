---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'SootDiff: Bytecode Comparison across Different Java Compilers'
subtitle: ''
summary: ''
authors:
- Andreas Dann
- Ben Hermann
- Eric Bodden
tags:
- Intermediate Representation
- Code Clone Detection
- Static Analysis
categories: []
date: '2019-01-01'
lastmod: 2022-01-10T09:51:49+01:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2022-01-10T08:51:48.955683Z'
publication_types:
- '1'
abstract: Different Java compilers and compiler versions, e.g., javac or ecj, produce
  different bytecode from the same source code. This makes it hard to trace if the
  bytecode of an open-source library really matches the provided source code. Moreover,
  it prevents one from detecting which open-source libraries have been re-compiled
  and rebundled into a single jar, which is a common way to distribute an application.
  Such rebundling is problematic because it prevents one to check if the jar file
  contains open-source libraries with known vulnerabilities. To cope with these problems,
  we propose the tool SootDiff that uses Soot's intermediate representation Jimple,
  in combination with code clone detection techniques, to reduce dissimilarities introduced
  by different compilers, and to identify clones. Our results show that SootDiff successfully
  identifies clones in 102 of 144 cases, whereas bytecode comparison succeeds in 58
  cases only.
publication: '*Proceedings of the 8th ACM SIGPLAN International Workshop on State
  Of the Art in Program Analysis*'
doi: 10.1145/3315568.3329966
links:
- name: URL
  url: https://doi.org/10.1145/3315568.3329966
---
