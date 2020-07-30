## Background
I co-teach an advanced placement computer science class at Heights High School in Houston with the TEALS program. The curriculum utilizes the Java programming language and has an emphasis on object-oriented programming. From a school IT system perspective, we have limited options for the software we can distribute to the students' laptops. During my first year of volunteering, we opted to use BlueJ for the first couple of months before exposing them to Eclipse, a more heavy-duty integrated development environment. Both editors have their challenges and limitations for novices, so we began to evaluate several other options, including Visual Studio Code. After considering numerous factors, including the complexity of installation, editor features, and accessibility, we opted to try a radically different option: Repl.it.

## Benefits and Implications
Repl.it is a feature-rich, browser-based IDE with support for numerous programming languages, including Java. In addition to the editor and computing environment, the application supports classroom features such as creating assignments that I will detail further below. Since Repl.it runs in the browser, there's no installation or configuration in terms of editors, runtimes, etc. Using a browser-based tool decreased the number of local support issues that we had to address. We found that students had much fewer problems with getting acclimated to the tooling compared to BlueJ and Eclipse. The user interface proved to be intuitive. There were relatively few issues with the underlying runtimes and virtualization that Repl.it abstracts from the user.

Repl.it requires an internet connection, and teachers shouldn't assume that students have internet access at home. Though many classes will be online due to the COVID-19 global pandemic, keep in mind that your students may have limited connectivity. I recommend offering desktop IDEs as an offline alternative so that students can at least run code locally.

## Setting Up a Classroom
TBD

## Integrating with GitHub
`.editorconfig`
```shell script
root = true

[*]
indent_style = tab
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
```

`.replit`
```shell script
language = "java10"
run = "javac Main.java && java Main"
```

## Repl.it