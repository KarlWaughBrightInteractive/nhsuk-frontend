# Action link

Find out more about the action link component and when to use it in the [NHS Digital service manual](https://beta.nhs.uk/service-manual/).

## Example

[Preview the action link component]()

## HTML markup

    <div class="nhsuk-action-link">
      <a href="https://www.nhs.uk/service-search/minor-injuries-unit/locationsearch/551" class="nhsuk-action-link__link">
        <svg class="nhsuk-icon nhsuk-icon__arrow-right-circle" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
          <path d="M0 0h24v24H0z" fill="none"/>
          <path d="M12 2a10 10 0 0 0-9.95 9h11.64L9.74 7.05a1 1 0 0 1 1.41-1.41l5.66 5.65a1 1 0 0 1 0 1.42l-5.66 5.65a1 1 0 0 1-1.41 0 1 1 0 0 1 0-1.41L13.69 13H2.05A10 10 0 1 0 12 2z"/>
        </svg>
        <span class="nhsuk-action-link__text">Find a minor injuries unit</span>
      </a>
    </div>

## Nunjucks macro

    {% from 'components/action-link/macro.njk' import actionLink %}

    {{ actionLink({
      "URL": "https://www.nhs.uk/service-search/minor-injuries-unit/locationsearch/551",
      "text": "Find a minor injuries unit"
    }) }}