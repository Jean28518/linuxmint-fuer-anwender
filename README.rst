How to build pdf and html locally:
----------------------------------

.. code-block:: shell

    # Debian/Ubuntu dependencies:
    sudo apt-get install texlive-latex-recommended texlive-latex-extra texlive-fonts-recommended latexmk texlive-xetex python3-sphinx-rtd-theme
    # Arch Linux dependencies:
    sudo pacman -S texlive-latexextra texlive-fontsrecommended texlive-xetex python-sphinx_rtd_theme texlive-bin texlive-latexmk
    
    cd docs

    rm -r build
    
    # Build PDF (optional, skip if you only want HTML):
    make latexpdf
    
    # Package everything (creates build/linuxmint-fuer-anwender.zip containing HTML and PDF):
    make dist

    PASSWORD=$(pwgen 8 1)

    cp build/linuxmint-fuer-anwender.zip build/linuxmint-fuer-anwender_${PASSWORD}.zip


