---
title: Table
keywords: table
sidebar: left-navigation-sidebar
toc: false
permalink: components/table.html
folder: components
---

A table is a set tabular data. Line items can support data, images and actions.

<hr />

## Default Table
The header columns allows the user to easily understand the data represented.

{% capture table-icon %}
<table class="fd-table">
    <thead>
        <tr>
            <th></th>
            <th>Column Header</th>
            <th>Column Header</th>
            <th>Column Header</th>
            <th>Column Header</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><span class=" fd-image--s fd-image--circle" aria-label="Image label"
            style="background-image: url(http://api.adorable.io/avatars/50/rodney.artichoke@hybris.com.png);">
            </span></td>
            <td><a href="#" class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>Last Name</td>
            <td>01/26/17</td>
        </tr>
        <tr>
            <td><span class=" fd-image--s fd-image--circle" aria-label="Image label"
            style="background-image: url(http://api.adorable.io/avatars/50/rodney.artichoke@hybris.com.png);">
            </span></td>
            <td><a href="#" class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>Last Name</td>
            <td>01/26/17</td>
        </tr>
        <tr>
            <td><span class=" fd-image--s fd-image--circle" aria-label="Image label"
            style="background-image: url(http://api.adorable.io/avatars/50/rodney.artichoke@hybris.com.png);">
            </span></td>
            <td><a href="#" class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>Last Name</td>
            <td>01/26/17</td>
        </tr>
    </tbody>
</table>
{% endcapture %}
{% include display-component.html component=table-icon %}

<br />

## Table with checkbox
The checkbox input can be used at the beginning of each row to allow for bulk actions.
It is recommended to add the parameter `area-selected="true` to the row that is selected.

{% capture table-checkbox %}
<table class="fd-table">
    <thead>
        <tr>
            <th><input type="checkbox"></th>
            <th>Column Header</th>
            <th>Column Header</th>
            <th>Column Header</th>
            <th>Column Header</th>
        </tr>
    </thead>
    <tbody>
        <tr aria-selected="true">
            <td><input type="checkbox" checked></td>
            <td><a class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>Last Name</td>
            <td>01/26/17</td>
        </tr>
        <tr>
            <td><input type="checkbox"></td>
            <td><a class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>Last Name</td>
            <td>01/26/17</td>
        </tr>
        <tr>
            <td><input type="checkbox"></td>
            <td><a class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>Last Name</td>
            <td>01/26/17</td>
        </tr>
    </tbody>
</table>
{% endcapture %}
{% include display-component.html component=table-checkbox %}

<br />

## Table with Contextual Menu
When more than three actions exist per row and/or space doesn't allow for actions,
a contextual menu can be substituted in order to display all actions in one menu.

{% capture table-actions %}
<table class="fd-table">
    <thead>
        <tr>
            <th>Column Header</th>
            <th>Column Header</th>
            <th>Column Header</th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><a class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>01/26/17</td>
            <td>
                <div class="fd-popover">
                    <div class="fd-popover__control">
                        <button class="fd-button--light sap-icon--vertical-grip" aria-controls="pQqQR213" aria-haspopup="true" aria-expanded="false" aria-label="More"></button>
                    </div>
                    <div class="fd-popover__body" aria-hidden="true" id="pQqQR213">
                        <nav class="fd-menu">
                            <ul class="fd-menu__list">
                                <li><a href="#" class="fd-menu__item">Edit</a></li>
                                <li><a href="#" class="fd-menu__item">Lock</a></li>
                                <li><a href="#" class="fd-menu__item">Duplicate</a></li>
                                <li><a href="#" class="fd-menu__item">Delete</a></li>
                            </ul>
                        </nav>
                    </div>
                </div>
            </td>
        </tr>
        <tr>
            <td><a class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>01/26/17</td>
            <td>
                <div class="fd-popover">
                    <div class="fd-popover__control">
                        <button class="fd-button--light sap-icon--vertical-grip" aria-controls="lkjlkj23" aria-haspopup="true" aria-expanded="false" aria-label="More"></button>
                    </div>
                    <div class="fd-popover__body" aria-hidden="true" id="lkjlkj23">
                        <nav class="fd-menu">
                            <ul class="fd-menu__list">
                                <li><a href="#" class="fd-menu__item">Edit</a></li>
                                <li><a href="#" class="fd-menu__item">Lock</a></li>
                                <li><a href="#" class="fd-menu__item">Duplicate</a></li>
                                <li><a href="#" class="fd-menu__item">Delete</a></li>
                            </ul>
                        </nav>
                    </div>
                </div>
            </td>
        </tr>
        <tr>
            <td><a class="fd-has-font-weight-semi">user.name@email.com</a></td>
            <td>First Name</td>
            <td>01/26/17</td>
            <td>
                <div class="fd-popover">
                    <div class="fd-popover__control">
                        <button class="fd-button--light sap-icon--vertical-grip" aria-controls="uu4324" aria-haspopup="true" aria-expanded="false" aria-label="More"></button>
                    </div>
                    <div class="fd-popover__body" aria-hidden="true" id="uu4324">
                        <nav class="fd-menu">
                            <ul class="fd-menu__list">
                                <li><a href="#" class="fd-menu__item">Edit</a></li>
                                <li><a href="#" class="fd-menu__item">Lock</a></li>
                                <li><a href="#" class="fd-menu__item">Duplicate</a></li>
                                <li><a href="#" class="fd-menu__item">Delete</a></li>
                            </ul>
                        </nav>
                    </div>
                </div>
            </td>
        </tr>
    </tbody>
</table>
{% endcapture %}
{% include display-component.html component=table-actions %}

<br />

## Table with Sortable Column Headers
{% capture table-sort %}
<table class="fd-table">
   <thead>
      <tr>
         <th class="fd-table__sort-column">Header Column</th>
         <th class="fd-table__sort-column">Header Column</th>
         <th class="fd-table__sort-column">Header Column</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
   </tbody>
</table>
{% endcapture %}
{% include display-component.html component=table-sort %}

<br>

## Table with Sortable Column Headers - Ascending
{% capture table-sort %}
<table class="fd-table">
   <thead>
      <tr>
         <th class="fd-table__sort-column fd-table__sort-column--asc">Header Column</th>
         <th class="fd-table__sort-column">Header Column</th>
         <th class="fd-table__sort-column">Header Column</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
   </tbody>
</table>
{% endcapture %}
{% include display-component.html component=table-sort %}

<br>

## Table with Sortable Column Headers - Descinding
{% capture table-sort %}
<table class="fd-table">
   <thead>
      <tr>
         <th class="fd-table__sort-column fd-table__sort-column--dsc">Header Column</th>
         <th class="fd-table__sort-column ">Header Column</th>
         <th class="fd-table__sort-column ">Header Column</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
   </tbody>
</table>
{% endcapture %}
{% include display-component.html component=table-sort %}

<br>

## Table with Column Headers with context menu
{% capture table-sort %}
<table class="fd-table">
   <thead>
      <tr>
         <th class="fd-table__context-menu " style="left:; width:"  aria-controls="col1" aria-haspopup="true" >
            <div class="fd-popover">
               <div class="fd-popover__control">
                  <span class="fd-table__context-menu-label">Header Column</span>
               </div>
               <div class="fd-popover__body"  aria-hidden="true" id="col1">
                  <nav class="fd-menu fd-menu--addon-before">
                     <ul class="fd-menu__list">
                        <li><a href="#" class="fd-menu__item">Ascending</a>
                        </li>
                        <li><a href="#" class="fd-menu__item">Decensing</a>
                        </li>
                        <hr>
                        <li><a href="#" class="fd-menu__item">Fix Column</a>
                        </li>
                     </ul>
                  </nav>
               </div>
            </div>
         </th>
         <th class="fd-table__context-menu " style="left:; width:"  aria-controls="col2" aria-haspopup="true" >
            <div class="fd-popover">
               <div class="fd-popover__control">
                  <span class="fd-table__context-menu-label">Header Column</span>
               </div>
               <div class="fd-popover__body"  aria-hidden="true" id="col2">
                  <nav class="fd-menu fd-menu--addon-before">
                     <ul class="fd-menu__list">
                        <li><a href="#" class="fd-menu__item">Ascending</a>
                        </li>
                        <li><a href="#" class="fd-menu__item">Decensing</a>
                        </li>
                        <hr>
                        <li><a href="#" class="fd-menu__item">Fix Column</a>
                        </li>
                     </ul>
                  </nav>
               </div>
            </div>
         </th>
         <th class="fd-table__context-menu " style="left:; width:"  aria-controls="col3" aria-haspopup="true" >
            <div class="fd-popover">
               <div class="fd-popover__control">
                  <span class="fd-table__context-menu-label">Header Column</span>
               </div>
               <div class="fd-popover__body"  aria-hidden="true" id="col3">
                  <nav class="fd-menu fd-menu--addon-before">
                     <ul class="fd-menu__list">
                        <li><a href="#" class="fd-menu__item">Ascending</a>
                        </li>
                        <li><a href="#" class="fd-menu__item">Decensing</a>
                        </li>
                        <hr>
                        <li><a href="#" class="fd-menu__item">Fix Column</a>
                        </li>
                     </ul>
                  </nav>
               </div>
            </div>
         </th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
         <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
      <tr>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
          <td>Lorem ipsum dolor sit amet ipsum</td>
      </tr>
   </tbody>
</table>
{% endcapture %}
{% include display-component.html component=table-sort %}

<br>

## Table with Fix Column Header and context menu
{% capture table-sort %}
<div class="fd-table--fixed-wrapper" style="width:800px;">
   <div class="fd-table--fixed">
      <table class="fd-table">
         <thead>
            <tr>
               <th class="fd-table__context-menu  fd-table__fixed-col" style="left:0; width:200px"  aria-controls="col1.2" aria-haspopup="true" >
                  <div class="fd-popover">
                     <div class="fd-popover__control">
                        <span class="fd-table__context-menu-label">Header Column</span>
                     </div>
                     <div class="fd-popover__body"  aria-hidden="true" id="col1.2">
                        <nav class="fd-menu fd-menu--addon-before">
                           <ul class="fd-menu__list">
                              <li>
                                 <div class="fd-menu__addon-before"></div>
                                 <a href="#" class="fd-menu__item">Ascending</a>
                              </li>
                              <li>
                                 <div class="fd-menu__addon-before"></div>
                                 <a href="#" class="fd-menu__item">Decensing</a>
                              </li>
                              <hr>
                              <li>
                                 <div class="fd-menu__addon-before"><span class="sap-icon--accept"></span></div>
                                 <a href="#" class="fd-menu__item">Fix Column</a>
                              </li>
                           </ul>
                        </nav>
                     </div>
                  </div>
               </th>
               <th class="fd-table__context-menu " style="left:200px; width:"  aria-controls="col2.2" aria-haspopup="true" >
                  <div class="fd-popover">
                     <div class="fd-popover__control">
                        <span class="fd-table__context-menu-label">Header Column</span>
                     </div>
                     <div class="fd-popover__body"  aria-hidden="true" id="col2.2">
                        <nav class="fd-menu fd-menu--addon-before">
                           <ul class="fd-menu__list">
                              <li><a href="#" class="fd-menu__item">Ascending</a>
                              </li>
                              <li><a href="#" class="fd-menu__item">Decensing</a>
                              </li>
                              <hr>
                              <li><a href="#" class="fd-menu__item">Fix Column</a>
                              </li>
                           </ul>
                        </nav>
                     </div>
                  </div>
               </th>
               <th class="fd-table__context-menu " style="left:; width:"  aria-controls="col3.2" aria-haspopup="true" >
                  <div class="fd-popover">
                     <div class="fd-popover__control">
                        <span class="fd-table__context-menu-label">Header Column</span>
                     </div>
                     <div class="fd-popover__body"  aria-hidden="true" id="col3.2">
                        <nav class="fd-menu fd-menu--addon-before">
                           <ul class="fd-menu__list">
                              <li><a href="#" class="fd-menu__item">Ascending</a>
                              </li>
                              <li><a href="#" class="fd-menu__item">Decensing</a>
                              </li>
                              <hr>
                              <li><a href="#" class="fd-menu__item">Fix Column</a>
                              </li>
                           </ul>
                        </nav>
                     </div>
                  </div>
               </th>
               <th class=" ">Header Column</th>
               <th class=" ">Header Column</th>
               <th class=" ">Header Column</th>
               <th class=" ">Header Column</th>
               <th class=" ">Header Column</th>
               <th class=" ">Header Column</th>
               <th class=" ">Header Column</th>
            </tr>
         </thead>
         <tbody>
            <tr>
               <td class="fd-table__fixed-col" style="left:0; width:200px">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:200px; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
            </tr>
            <tr>
               <td class="fd-table__fixed-col" style="left:0; width:200px">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:200px; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
            </tr>
            <tr>
               <td class="fd-table__fixed-col" style="left:0; width:200px">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:200px; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
               <td class="" style="left:; width:">Lorem ipsum dolor sit amet ipsum</td>
            </tr>
         </tbody>
      </table>
   </div>
</div>
{% endcapture %}
{% include display-component.html component=table-sort %}
