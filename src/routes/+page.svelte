<script>
  import "../lib/index";
  import * as j from "jquery";

  var dogs = [
    "Afghan Hound",
    "Chinese Crested",
    "Anatolian Shepherd Dog",
    "Basenji",
    "Black Russian Terrier",
    "Borzoi",
    "Cane Corso",
    "Chinese Shar-Pei",
    "Komondor",
    "Neapolitan Mastiff",
    "Puli",
    "Tibetan Mastiff",
    "Chihuahua",
    "Dachshund",
    "Italian Greyhound",
    "Pekingese",
    "Xoloitzcuintli",
    "American Pit Bull Terrier",
    "American Staffordshire Terrier",
    "Dalmatian",
    "American Eskimo Dog",
    "Chow Chow",
    "Eskimo Dog",
    "Keeshond",
    "Shiba Inu",
    "Bichon Frise",
    "Cavalier King Charles Spaniel",
    "Clumber Spaniel",
    "Cotondetulear",
    "English Toy Spaniel",
    "Havanese",
    "Japanese Chin",
    "King Charles Spaniel",
    "Lhasa Apso",
    "Löwchen",
    "Maltese",
    "Papillon",
    "Pomeranian",
    "Schipperke",
    "Shih Tzu",
    "Silky Terrier",
    "Soft-Coated Wheaten Terrier",
    "Sussex Spaniel",
    "Tibetan Spaniel",
    "Yorkshire Terrier",
    "Brussels Griffon",
    "Basset Hound",
    "Bloodhound",
    "Boston Terrier",
    "Bulldog",
    "English Bulldog",
    "French Bulldog",
    "Greyhound",
    "Mastiff",
    "Pug",
    "Saluki",
    "Sloughi",
    "Toy Fox Terrier",
    "Whippet",
    "Affenpinscher",
    "Bedlington Terrier",
    "Cairn Terrier",
    "Dandie Dinmont Terrier",
    "Glen of Imaal Terrier",
    "Irish Terrier",
    "Kerry Blue Terrier",
    "Lakeland Terrier",
    "Norfolk Terrier",
    "Norwich Terrier",
    "Otterhound",
    "Scottish Terrier",
    "Sealyham Terrier",
    "Skye Terrier",
    "Welsh Terrier",
    "West Highland White Terrier",
    "Wire Fox Terrier",
    "Akita",
    "American Bulldog",
    "American Cocker Spaniel",
    "American Foxhound",
    "American Water Spaniel",
    "Australian Terrier",
    "Beagle",
    "Bernese Mountain Dog",
    "Black and Tan Coonhound",
    "Border Terrier",
    "Boykin Spaniel",
    "Brittany",
    "Bull Terrier",
    "Bullmastiff",
    "Cardigan Welsh Corgi",
    "Cockapoo",
    "Coonhound",
    "Corgi",
    "Dogo Argentino",
    "English Cocker Spaniel",
    "English Foxhound",
    "Great Dane",
    "Great Pyrenees",
    "Harrier",
    "Irish Wolfhound",
    "Jack Russell Terrier",
    "Manchester Terrier",
    "Miniature Bull Terrier",
    "Miniature Pinscher",
    "Newfoundland",
    "Norwegian Lundehund",
    "Old English Sheepdog",
    "Pembroke Welsh Corgi",
    "Petit Basset Griffon Vendeen",
    "Pharaoh Hound",
    "Plott",
    "Presa Canario",
    "Rat Terrier",
    "Redbone Coonhound",
    "Saint Bernard",
    "Samoyed",
    "Scottish Deerhound",
    "Shetland Sheepdog",
    "Staffordshire Bull Terrier",
    "Tibetan Terrier",
    "Treeing Walker Coonhound",
    "Airedale Terrier",
    "Alaskan Malamute",
    "Australian Cattle Dog",
    "Australian Shepherd",
    "Bearded Collie",
    "Belgian Malinois",
    "Belgian Sheepdog",
    "Belgian Tervuren",
    "Border Collie",
    "Bouvier des Flandres",
    "Boxer",
    "Briard",
    "Chesapeake Bay Retriever",
    "Collie",
    "Curly-Coated Retriever",
    "Doberman Pinscher",
    "Dutch Shepherd",
    "English Setter",
    "English Springer Spaniel",
    "Entlebucher Mountain Dog",
    "Field Spaniel",
    "Finnish Lapphund",
    "Finnish Spitz",
    "Flat-Coated Retriever",
    "German Pinscher",
    "German Shepherd Dog",
    "German Shorthaired Pointer",
    "German Wirehaired Pointer",
    "Giant Schnauzer",
    "Goldador",
    "Golden Retriever",
    "Goldendoodle",
    "Gordon Setter",
    "Greater Swiss Mountain Dog",
    "Irish Setter",
    "Irish Water Spaniel",
    "Klee Kai",
    "Kuvasz",
    "Labrador Retriever",
    "Lagotto Romagnolo",
    "Maremma Sheepdog",
    "Miniature Schnauzer",
    "Norwegian Buhund",
    "Norwegian Elkhound",
    "Nova Scotia Duck Tolling Retriever",
    "Pointer",
    "Polish Lowland Sheepdog",
    "Poodle",
    "Portuguese Water Dog",
    "Pumi",
    "Pyrenean Shepherd",
    "Rhodesian Ridgeback",
    "Rottweiler",
    "Siberian Husky",
    "Small Munsterlander Pointer",
    "Spanish Water Dog",
    "Spinone Italiano",
    "Standard Schnauzer",
    "Swedish Vallhund",
    "Vizsla",
    "Weimaraner",
    "Welsh Springer Spaniel",
    "Wirehaired Pointing Griffon",
    "Wirehaired Vizsla",
  ];

  var properties = [
    {
      Price: "$255,000",
      Address1: "2150 Anderson Rd UNIT 1602",
      Address2: "Oxford, MS 38655",
      HomeType: "Multi Family Residence",
      Bedrooms: "2 Bd",
      Baths: "3 Ba",
      SqFt: "1,142 sqft",
      Image: "Anderson.jpg",
      Score: 51,
    },
    {
      Price: "$257,500",
      Address1: "210 Private Road 3049",
      Address2: "Oxford, MS 38655",
      HomeType: "Single Family Residence",
      Bedrooms: "3 Bd",
      Baths: "3 Ba",
      SqFt: "1,340 sqft",
      Image: "210PR.jpg",
      Score: 59,
    },
    {
      Price: "$229,900",
      Address1: "2109 Harris Dr UNIT 25",
      Address2: "Oxford, MS 38655",
      HomeType: "Multi Family Residence",
      Bedrooms: "2 Bd",
      Baths: "3 Ba",
      SqFt: "1,120 sqft",
      Image: "Harris.jpg",
      Score: 65,
    },
    {
      Price: "$279,000",
      Address1: "213 Sweet Bay Dr",
      Address2: "Oxford, MS 38655",
      HomeType: "Single Family Residence",
      Bedrooms: "3 Bd",
      Baths: "3 Ba",
      SqFt: "1,500 sqft",
      Image: "SweetBay.jpg",
      Score: 68,
    },
    {
      Price: "$499,900",
      Address1: "124 Hillside Dr",
      Address2: "Oxford, MS 38655",
      HomeType: "Single Family Residence",
      Bedrooms: "5 Bd",
      Baths: "3 Ba",
      SqFt: "3,290 sqft",
      Image: "HillSide.jpg",
      Score: 81,
    },
    {
      Price: "$1,050,000",
      Address1: "232 Saint Andrews Cir",
      Address2: "Oxford, MS 38655",
      HomeType: "Single Family Residence",
      Bedrooms: "4 Bd",
      Baths: "5 Ba",
      SqFt: "6,375 sqft",
      Image: "SaintAndrews.jpg",
      Score: 85,
    },
  ];

  var filteredProps = properties;
  var mapImage = "Map-all.png";
  var showImage = false;
  function handleClick() {
    let selected = document.getElementById("demoAutocomplete1").value;
    if (selected !== "Chihuahua") {
      mapImage = "Map-One.png";
      filteredProps = properties.filter((x) => x.Score >= 85);
    } else {
      mapImage = "Map-all.png";
      filteredProps = properties;
    }
    showImage = true;
  }

  j(document).ready(function () {
    console.log(window.CLUI);
    window.CLUI.autoCompleteInit("#demoAutocomplete1", { list: dogs });
  });
</script>

<div class="container-fluid">
  <nav
    class="cl-main-nav navbar navbar-dark navbar-expand-md"
    style="margin-bottom: 1rem;"
  >
    <a href="#" class="navbar-brand"
      ><span class="navbar-logo" />Pawsitive Solutions</a
    >
    <div class="navbar-toggler">
      <nav aria-labelledby="navbarMobileToggler" class="nav">
        <a
          id="navbarMobileToggler"
          aria-expanded="false"
          data-toggle="collapse"
          href="#navbarSupportedContent"
          class="nav-item nav-link collapsed menu-toggle"
          ><span class="fa fa-bars"
            ><span class="sr-only">Toggle Navigation</span></span
          ></a
        >
      </nav>
    </div>
    <div id="navbarSupportedContent" class="navbar-collapse collapse" />
  </nav>
  <div class="form-group custom-autocomplete">
    <label for="demoAutocomplete1">Select your dog breed</label>
    <div class="input-group left-icon">
      <span class="input-group-addon input-icon">
        <span class="fa fa-search" /></span
      >
      <input
        type="text"
        id="demoAutocomplete1"
        class="form-control"
        placeholder="Search for a dog breed"
        aria-expanded="false"
        aria-owns="awesomplete_list_2"
        role="combobox"
        on:blur={() => handleClick()}
      />
    </div>
  </div>
  <div style="text-align: center;">
    {#if showImage}
      <img src={mapImage} alt="" style="margin-bottom: 1rem;" />
      <!-- https://www.tutorialspoint.com/how-to-convert-speech-to-text-using-javascript -->
      <div class="container-fluid">
        <div class="property-card-container" style="justify-content: center;">
          {#each filteredProps as prop}
            <div class="card property-card shadow">
              <div
                class="property-photo"
                style="background-image: url({prop.Image});"
              />
              <div class="card-body">
                <div class="status-row">
                  <div class="property-status for-sale">For Sale</div>
                  <div class="ml-auto">
                    <span>🐶</span>
                    <span>{prop.Score}</span>
                  </div>
                </div>
                <h2 class="property-title">{prop.Price}</h2>
                <div class="property-subtitle">{prop.HomeType}</div>
                <address>{prop.Address1}<br />{prop.Address2}</address>
                <div class="attribute-row">
                  <div class="attribute">{prop.Bedrooms}</div>
                  <div class="attribute">{prop.Baths}</div>
                  <div class="attribute">{prop.SqFt}</div>
                </div>
              </div>
            </div>
          {/each}
        </div>
      </div>
    {/if}
  </div>
  <footer class={showImage ? 'footer footer-dark footer-big' : 'footer footer-dark footer-small'}>
    <div class="footer-logo">
      <div class="clgx-logo" />
    </div>
    <div class="footer-nav">
      <ul class="nav">
        <li class="nav-item">
          <a href="javascript:" class="nav-link">About Our Company</a>
        </li>
        <li class="nav-divider" />
        <li class="nav-item">
          <a href="javascript:" class="nav-link">Contact Us</a>
        </li>
        <li class="nav-divider" />
        <li class="nav-item">
          <a href="javascript:" class="nav-link">FAQs</a>
        </li>
        <li class="nav-divider" />
        <li class="nav-item">
          <a href="javascript:" class="nav-link">Sitemap</a>
        </li>
        <li class="nav-divider" />
        <li class="nav-item">
          <a
            href="https://www.corelogic.com/legal.aspx"
            target="_blank"
            class="nav-link">Legal</a
          >
        </li>
        <li class="nav-divider" />
        <li class="nav-item">
          <a
            href="https://www.corelogic.com/privacy.aspx"
            target="_blank"
            class="nav-link">Privacy</a
          >
        </li>
      </ul>
      <div class="footer-date">© 2023 CoreLogic. All Rights Reserved.</div>
    </div>
  </footer>
</div>


<style>
    .footer-big {
        margin-top: 1rem;
    }

    .footer-small {
        margin-top: 450px;
    }
</style>