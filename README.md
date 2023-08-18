# CV

## Credit

- Simple and Clear Your Username Resume: https://www.overleaf.com/latex/templates/simple-and-clear-your-username-resume/wksqncvzcbff

## History

### Do not Uppercase

We do not transform `\name` to uppercases and increase the font size (`\huge` to `\Huge`).

```latex
% \printname is used to print the name as a page header
\def \printname {
  \begingroup
    \hfil{{\namesize\bf \@name}}\hfil
%    \hfil{\MakeUppercase{\namesize\bf \@name}}\hfil
    \nameskip\break
  \endgroup
}

% The below commands define the whitespace after certain things in the document - they can be \smallskip, \medskip or \bigskip
\def\namesize{\Huge} % Size of the name at the top of the document
%\def\namesize{\huge} % Size of the name at the top of the document
\def\addressskip{\smallskip} % The space between the two address (or phone/email) lines
\def\sectionlineskip{\medskip} % The space above the horizontal line for each section 
\def\nameskip{\bigskip} % The space after your name at the top
\def\sectionskip{\medskip} % The space after the heading section
```
