---
layout: default
title: Reverie Romantique - Portfolio
---
# Portfolio
<br>
<h4>These are products that Reverie Romantique have created in the past. We hope to make them available to you shortly!</h4>
<br>
<div class="container">
    <div class="row">
        {% for product in site.data.product_info %}
        <div class="col-md-6 gallery-item">
            <a href="products/{{ product.link }}">
                <img src="/assets/products/{{ product.image }}" class="img-fluid img-responsive img-rounded">
            </a>
            <div class="product-card"><a href="products/{{ product.link }}" class="product-link">{{ product.name }}</a></div>
            <div class ="product-subtitle">{{ product.description }}</div>
        </div> 
        {% endfor %}
    </div>
</div>


