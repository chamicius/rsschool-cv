#Пупкин Василий Васильевич
dsgffrg@rt.by **(29) 125-25-25**
Skills:
* HTML5
* CSS3
* JQuery
My code example:
```
<?php $_helper = $this->helper('catalog/output'); ?>
<?php $_product = $this->getProduct(); ?>
<script type="text/javascript">
    var optionsPrice = new Product.OptionsPrice(<?php echo $this->getJsonConfig() ?>);
</script>
<div id="messages_product_view"><?php echo $this->getMessagesBlock()->toHtml() ?></div>
<div class="product-view">
    <div class="product-essential flex-column-reverse flex-sm-row">
        <div class="d-flex flex-column-reverse flex-sm-column">
        <form action="<?php echo $this->getSubmitUrl($_product, array('_secure' => $this->_isSecure())) ?>" method="post" id="product_addtocart_form"<?php if($_product->getOptions()): ?> enctype="multipart/form-data"<?php endif; ?>>
            <?php echo $this->getBlockHtml('formkey') ?>
            <div class="no-display">
                <input type="hidden" name="product" value="<?php echo $_product->getId() ?>" />
                <input type="hidden" name="related_product" id="related-products-field" value="" />
            </div>
            <div class="container">
                <div class="row">
                    <div class="order-1 order-sm-0 product-name col-12 col-md-12 row">
                        <div class="product-name col-12 col-md-6">
                            <span class="h1"><?php echo $_helper->productAttribute($_product, $_product->getName(), 'name') ?></span>
                            <?php echo $this->getChildHtml('product_type_availability'); ?>
                        </div>
```
English level: *Intermediate *




