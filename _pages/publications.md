// _sass/publications.scss

// --------------------------------------------------
// Sticky masthead
// --------------------------------------------------

.masthead {
  position: sticky;
  top: 0;
  background: rgba(255, 255, 255, 0.97);
  backdrop-filter: blur(6px);
  z-index: 999;
}

// --------------------------------------------------
// Pull publications content to align with masthead
// The contrast skin adds excess left padding on wide
// layout — this corrects it without touching the
// outer wrapper's width or breaking responsiveness
// --------------------------------------------------

.layout--single.wide .page__content,
.page__content {
  padding-left: 0;
  padding-right: 0;
}

// --------------------------------------------------
// Publications wrapper
// --------------------------------------------------

.pubs {
  font-size: 0.88rem;
  line-height: 1.65;
  max-width: 680px; // keeps line length readable
}

// --------------------------------------------------
// Category block
// --------------------------------------------------

.pub-row {
  display: block;
  margin-bottom: 3rem;
  padding-top: 1.6rem;
  border-top: 1px solid #e0e0e0;

  &:first-child {
    border-top: none;
    padding-top: 0;
  }
}

// --------------------------------------------------
// Category label — small, grey, uppercase
// --------------------------------------------------

.pub-type {
  font-size: 0.68rem;
  color: #999;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  margin-bottom: 1.4rem;
  font-weight: 400;
}

// --------------------------------------------------
// Year headings — slightly larger than body,
// clearly separated from the category label
// --------------------------------------------------

.pubs strong {
  display: block;
  font-size: 0.78rem;
  font-weight: 600;
  color: #333;
  margin-top: 1.8rem;
  margin-bottom: 0.5rem;

  &:first-child {
    margin-top: 0;
  }
}

// --------------------------------------------------
// Individual entries
// --------------------------------------------------

.pub-list p {
  margin-bottom: 1rem;
}

// --------------------------------------------------
// Links — neutral, not the contrast skin's teal
// --------------------------------------------------

.pubs a {
  color: #222;
  text-decoration: none;
  border-bottom: 1px solid #bbb;
  transition: border-color 0.15s ease;

  &:hover {
    border-bottom-color: #222;
    color: #000;
  }

  &:visited {
    color: #444;
  }
}

// --------------------------------------------------
// Journal name
// --------------------------------------------------

.pubs em {
  color: #777;
  font-style: italic;
}

// --------------------------------------------------
// Responsive — on small screens restore some padding
// --------------------------------------------------

@media (max-width: 768px) {
  .layout--single.wide .page__content,
  .page__content {
    padding-left: 1rem;
    padding-right: 1rem;
  }

  .pubs {
    max-width: 100%;
  }
}
