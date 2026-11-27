# Cómo publicar el repositorio tras la defensa

Los repositorios de TFE son **privados** mientras dura el trabajo. Tras la defensa se hacen **públicos** para que el trabajo pueda consultarse, reutilizarse y citarse (ciencia abierta). Este proceso lo hacen juntos el alumno y el tutor.

## 1. Revisión previa

- [ ] **Sin credenciales:** ni contraseñas, ni tokens, ni claves (por ejemplo, usuario y contraseña de NTRIP o de wifi). Si alguna vez se subieron, **cámbialas** antes de publicar: aunque las borres, siguen en el historial de Git.
- [ ] **Sin datos personales** (DNI, teléfonos, correos personales) ni información confidencial de colaboradores.
- [ ] **Sin ficheros grandes** innecesarios (rosbags, vídeos, pesos de redes): enlázalos desde el README si hace falta.
- [ ] **README completo:** requisitos, instalación, uso, resultados.
- [ ] **Código de terceros:** comprueba que las licencias del código reutilizado son compatibles con Apache-2.0 y cítalo en el README (si partes de código GPL, el repositorio debe ser GPL).

## 2. Licencia, cita y DOI

1. **Licencia:** añade un fichero `LICENSE` con el texto de la [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt) y, al principio del README o en un fichero `NOTICE`, la línea `Copyright «año» «Nombre del autor»`. El autor es quien ha escrito el código; si el tutor ha escrito parte, figura también. La documentación y las figuras se publican con [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.es).
2. **Cita:** copia `docs/plantillas_publicacion/CITATION.cff` a la raíz del repositorio y complétalo. GitHub mostrará el botón *«Cite this repository»*.
3. **DOI con Zenodo:**
   - El autor inicia sesión en [zenodo.org](https://zenodo.org) con su cuenta de GitHub y activa este repositorio en *GitHub → Repositories* (o lo hace un mentor si el repositorio está en la organización).
   - Copia `docs/plantillas_publicacion/.zenodo.json` a la raíz y complétalo: el alumno como autor (*creator*) y el tutor como colaborador con el rol *Supervisor*.
4. **Haz público el repositorio** (*Settings → General → Danger Zone → Change visibility*; lo hace un mentor).
5. **Crea una release** `v1.0-defensa` (*Releases → Draft a new release*). Zenodo la archiva y genera el DOI; añade la insignia del DOI al README y cítalo en la memoria y en tu currículum.

## 3. Después

- Añade el trabajo a la tabla de TFE del perfil público de la organización (repositorio `.github`, fichero `profile/README.md`).
- Añade el enlace al histórico de TFE de la wiki del equipo.
