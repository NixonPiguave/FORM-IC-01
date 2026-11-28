# FORM-IC-01 - Investigación individual

## Tema

**Empresa:** Amazon.  
**Estilo:** arquitectura orientada a servicios (SOA).  
**Caso:** evolución de la plataforma de comercio electrónico Amazon.com desde una arquitectura monolítica hacia servicios independientes.

## Primer avance

Este avance contiene la delimitación del caso, su descripción y escala histórica, los antecedentes del cambio y los primeros beneficios y desafíos documentados. Las citas están gestionadas con `biblatex` en formato IEEE.

Las dos fuentes incluidas son documentos oficiales de Amazon y AWS. No sustituyen las dos referencias académicas de los últimos cinco años exigidas para la entrega final.

## Archivos

- `informe.tex`: archivo principal de LaTeX.
- `referencias.bib`: bibliografía inicial del caso.
- `informe.pdf`: PDF compilado del avance, con una página de contenido y otra de referencias.
- `.gitignore`: exclusiones de archivos auxiliares de compilación.

## Compilación

**Compilador:** pdfLaTeX.  
**Gestor de bibliografía:** Biber.  
**Archivo principal:** `informe.tex`.

Desde la carpeta que contiene `informe.tex`, ejecutar en este orden:

```bash
pdflatex -interaction=nonstopmode -halt-on-error informe.tex
biber informe
pdflatex -interaction=nonstopmode -halt-on-error informe.tex
pdflatex -interaction=nonstopmode -halt-on-error informe.tex
```

### Dependencias

- TeX Live o MiKTeX con pdfLaTeX y Biber disponibles.
- Paquetes: `inputenc`, `fontenc`, `babel` con español, `lmodern`, `geometry`, `microtype`, `csquotes`, `biblatex`, `biblatex-ieee`, `hyperref` y `xurl`.

## Fuentes iniciales

1. [Amazon - 2010 Letter to Shareholders](https://www.sec.gov/Archives/edgar/data/1018724/000119312511110797/dex991.htm). La carta corresponde al ejercicio 2010 y se publicó en 2011. Documenta el uso de SOA y la intervención de entre 200 y 300 servicios para construir una página de producto.
2. [AWS - Cloud Enablement Engine: A Practical Guide](https://d1.awsstatic.com/whitepapers/cloud-enablement-engine-practical-guide.pdf). Versión del 14 de julio de 2021. El apéndice B, páginas impresas 17 a 20, describe la transformación de Amazon.com; comienza en la página 22 del archivo PDF.


El PDF de este primer avance se conserva en el repositorio. Para el SGA se preparará un documento separado con los datos identificativos y la URL completa del repositorio en una sola línea.