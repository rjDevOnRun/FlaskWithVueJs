TO RUN APPLICATION:

    - set FLASK_APP=app.py
    - python -m flask run

    or

    - in app.py bottom-most add:
        if __name__ == "__main__":
            app.run()
    - now use command to run:
        python app.py


TURN ON DEBUG MODE:
    - app.run(debug=True)


STATIC folder must contain all the 
styling related items

TEMPLATES folder must contain all the
html template pages for the application
    - python by default expects rendering
      html pages to be available in 'templates' folder


BOOTSTRAP:
    - www.getbootstrap.com
    - download 'compiled css & js'
    - save to 'static' folder
    - link to 'bootst...min.css'


    - startbootstrap.com
        - download a theme
        - overwrite the contents of 'static' folder
        - make sure to chage the 'src / href' to
          the correct location in your application
          i.e: ./static/xxxx folder....
        
TEMPLATE LINKING
    - move all template data to 'layout.html'
    - create seperate pages for each section
    - update the Nav-Bar link '#xxxx' -> '/xxxx'


VUE.js
    - add CDN ref to bottom of layout.html  
        <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    - define new 'delimiters' to allow Vue codes in html because 
      jinja also uses {{}} for its codes....
    