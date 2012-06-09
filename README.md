ZfcTwitterBootstrap
===================
Version 0.1.0 Created by Mike Willbanks

Introduction
------------

ZfcTwitterBootstrap is a module that attempts to handle Twitter Bootstrap
integration for Zend Framework 2.  Out of the box this presently includes
view helpers to render forms.  Overall this module will continue to grow
out the view helpers to assist in generating many of the items that Twitter
Bootstrap contains.

Requirements
------------

* [Zend Framework 2](https://github.com/zendframework/zf2) (latest master)

Features
--------
* Form Integration
  * FormRenderer
  * FormElement
  * FormDescription

Roadmap
-------

* Zend\Form - Completed basic integration
* Zend\Navigation - Not started
* Alert Messages - Not started

Usage
-----

    <?php
    // render a whole form
    echo $this->formRenderer($this->form);
    ?>


    <?php
    // render element by element
    $form = $this->form;
    $form->prepare();
    echo $this->form()->openTag($form);
    echo $this->formElement($this->form->get('element'));
    echo $this->form()->closeTag();
    ?>>
