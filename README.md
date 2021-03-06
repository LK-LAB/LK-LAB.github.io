lk-lab.github.io
==============
Forked form tech.kakao.com

> 주의: [GitHub Pages]와 [Jekyll]에 대해서 충분히 숙지할 것.
> 주의: [Collaborating on projects using issues and pull requests](https://help.github.com/categories/collaborating-on-projects-using-issues-and-pull-requests/)을 정독.


### 새 글 작성

1. `_drafts` 디렉토리에 `적당한이름.md` 이름으로 파일을 만들고
2. 포스트를 마크다운으로 작성
  - [gfm] 문법, [kramdown] 파서, [rouge] 문법강조기 사용
3. 확인 
```
$ bundle exec jekyll serve --drafts
```

### 글 쓰기

1. `_posts` 디렉토리에 `yyyy-mm-dd-slug.md` 파일로 복사(or 이동).
 - slug: 해당 포스트의 고유 키로 url의 일부로 사용. 왠만하면 특수문자없이 영문자,숫자,-(하이픈),.(점)...만 사용.
 - yyyy,mm,dd: 발행 년,월,일.
 - 참고: 최종적으로 포스트의 url(permalink)는 http://lk-lab.github.io/yyyy/mm/dd/slug/
2. 파일 상단에 [front matter] 작성
 - layout: post # 레이아웃(필수). `page` 레이아웃을 사용하면 목록에 보이지 않는 글을 쓸 수 있음.
 - title: '제목' # 제목(필수)
 - author: `lastname.firstname` # 필자(필수). 왠만하면 회사 아이디(예: iolo.fitzowen) 사용
 - tags: `[tag1,tag2,tag3,...]` # 태그 목록(선택). 왠만하면 특수문자없이 영소문자,숫자,-(하이픈),.(점)...만 사용.
 - image: http://... # 커버이미지 url(선택)
 - date: `YYYY-MM-DD HH:MM:SS` # 발행일(필수)
3. 처음 글을 쓰는 필자이라면 **글쓴이 등록**(필수)
4. 유력한(?) 태그가 새로 등장했다면 **태그 등록**(선택)

### 필자 등록

1. `_authors` 디렉토리에 `lastname.firstname.md` 이름으로 필자 정보 파일 추가
 - 참고: 최종적으로 사용자 포스트 목록 페이지의 url은 http://lk-lab.github.io/authors/lastname.firstname/
2. 파일 상단에 [front matter] 작성
 - layout: author # 레이아웃(필수)
 - name: `lastname.firstname` # post의 author와 매칭(필수). 왠만하면 회사 아이디(예: iolo.fitzowen) 사용. 왠만하면 특수문자없이 영소문자,숫자,-(하이픈),.(점)...만 사용.
 - title: ... # 왠만하면 한글이름 사용( 필수)
 - image: http://... # 프로필 이미지(필수)
 - cover: http://... # 작성자 커버 이미지(선택)
3. 내용은 필요없음

### 태그 등록

1. `_tags` 디렉토리에 `tag-name.md` 이름으로 필자 정보 파일 추가
 - 참고: 최종적으로 사용자 포스트 목록 페이지의 url은 http://lk-lab.github.io/tags/tag-name/
2. 파일 상단에 [front matter] 작성
 - layout: tag # 레이아웃(필수)
 - name: `tag-name` # post의 tags 배열의 항목과 매칭(필수). 왠만하면 특수문자없이 영소문자,숫자,-(하이픈),.(점)...만 사용.
 - title: ... # 좀 더 길고 구체적인 설명(필수)
 - image: http://... # 태그 이미지(선택)
3. 내용은 필요없음

---

문의: <dg981001@gmail.com>

May the **SOURCE** be with you...

[GitHub Pages]: https://pages.github.com
[Jekyll]: https://jekyllrb.com
[front matter]: https://jekyllrb.com/docs/frontmatter/
[gfm]: https://guides.github.com/features/mastering-markdown/
[kramdown]: http://kramdown.gettalong.org
[rouge]: http://rouge.jneen.net


## License

This software is licensed under the [Apache 2 license](LICENSE.txt), quoted below.

Copyright 2019 LK LAB. <http://lk-lab.github.io>

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this project except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
